# Comparing `tmp/gdmty_django_users-24.4.2.tar.gz` & `tmp/gdmty_django_users-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdmty_django_users-24.4.2.tar", last modified: Tue May  7 16:19:30 2024, max compression
+gzip compressed data, was "gdmty_django_users-24.5.0.tar", last modified: Fri May 10 04:33:08 2024, max compression
```

## Comparing `gdmty_django_users-24.4.2.tar` & `gdmty_django_users-24.5.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 16:19:30.108258 gdmty_django_users-24.4.2/
--rw-rw-rw-   0        0        0    35182 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.2/LICENSE
--rw-rw-rw-   0        0        0       51 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0    43751 2024-05-07 16:19:30.107252 gdmty_django_users-24.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     2100 2024-05-06 03:29:06.000000 gdmty_django_users-24.4.2/README.md
--rw-rw-rw-   0        0        0     1577 2024-05-07 16:19:03.000000 gdmty_django_users-24.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 16:19:30.109325 gdmty_django_users-24.4.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-07 16:19:30.052958 gdmty_django_users-24.4.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 16:19:30.086227 gdmty_django_users-24.4.2/src/gdmty_django_users/
--rw-rw-rw-   0        0        0     1368 2024-05-07 16:19:03.000000 gdmty_django_users-24.4.2/src/gdmty_django_users/__init__.py
--rw-rw-rw-   0        0        0     2478 2024-05-07 06:22:05.000000 gdmty_django_users-24.4.2/src/gdmty_django_users/admin.py
--rw-rw-rw-   0        0        0     1049 2024-05-07 06:22:05.000000 gdmty_django_users-24.4.2/src/gdmty_django_users/apps.py
--rw-rw-rw-   0        0        0     1438 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.2/src/gdmty_django_users/decorators.py
--rw-rw-rw-   0        0        0     2333 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.2/src/gdmty_django_users/managers.py
-drwxrwxrwx   0        0        0        0 2024-05-07 16:19:30.098719 gdmty_django_users-24.4.2/src/gdmty_django_users/migrations/
--rw-rw-rw-   0        0        0     3284 2024-03-17 01:44:29.000000 gdmty_django_users-24.4.2/src/gdmty_django_users/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.2/src/gdmty_django_users/migrations/__init__.py
--rw-rw-rw-   0        0        0     3205 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.2/src/gdmty_django_users/models.py
--rw-rw-rw-   0        0        0     1820 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.2/src/gdmty_django_users/permissions.py
--rw-rw-rw-   0        0        0     1764 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.2/src/gdmty_django_users/serializers.py
--rw-rw-rw-   0        0        0     1066 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.2/src/gdmty_django_users/settings.py
--rw-rw-rw-   0        0        0      911 2024-05-07 06:22:05.000000 gdmty_django_users-24.4.2/src/gdmty_django_users/tests.py
--rw-rw-rw-   0        0        0     1757 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.2/src/gdmty_django_users/urls.py
--rw-rw-rw-   0        0        0     4812 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.2/src/gdmty_django_users/viewsets.py
--rw-rw-rw-   0        0        0     1472 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.2/src/gdmty_django_users/wagtail_forms.py
-drwxrwxrwx   0        0        0        0 2024-05-07 16:19:30.103736 gdmty_django_users-24.4.2/src/gdmty_django_users.egg-info/
--rw-rw-rw-   0        0        0    43751 2024-05-07 16:19:30.000000 gdmty_django_users-24.4.2/src/gdmty_django_users.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      821 2024-05-07 16:19:30.000000 gdmty_django_users-24.4.2/src/gdmty_django_users.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 16:19:30.000000 gdmty_django_users-24.4.2/src/gdmty_django_users.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2024-05-07 16:19:30.000000 gdmty_django_users-24.4.2/src/gdmty_django_users.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-07 16:19:30.000000 gdmty_django_users-24.4.2/src/gdmty_django_users.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 04:33:08.703131 gdmty_django_users-24.5.0/
+-rw-rw-rw-   0        0        0    35182 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.0/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    43714 2024-05-10 04:33:08.703131 gdmty_django_users-24.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2113 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/README.md
+-rw-rw-rw-   0        0        0     1527 2024-05-10 04:32:53.000000 gdmty_django_users-24.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 04:33:08.703131 gdmty_django_users-24.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 04:33:08.671486 gdmty_django_users-24.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 04:33:08.692624 gdmty_django_users-24.5.0/src/gdmty_django_users/
+-rw-rw-rw-   0        0        0     1367 2024-05-10 04:32:53.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/__init__.py
+-rw-rw-rw-   0        0        0     2477 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/admin.py
+-rw-rw-rw-   0        0        0     1048 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/apps.py
+-rw-rw-rw-   0        0        0     1437 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/decorators.py
+-rw-rw-rw-   0        0        0     2332 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/managers.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:33:08.703131 gdmty_django_users-24.5.0/src/gdmty_django_users/migrations/
+-rw-rw-rw-   0        0        0     3284 2024-05-10 04:28:25.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1333 2024-05-10 04:29:08.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/migrations/0002_alter_user_groups_alter_user_user_permissions_and_more.py
+-rw-rw-rw-   0        0        0        0 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3204 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/models.py
+-rw-rw-rw-   0        0        0     1819 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/permissions.py
+-rw-rw-rw-   0        0        0     1763 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/serializers.py
+-rw-rw-rw-   0        0        0     1065 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/settings.py
+-rw-rw-rw-   0        0        0      910 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/tests.py
+-rw-rw-rw-   0        0        0     1756 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/urls.py
+-rw-rw-rw-   0        0        0     4811 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/viewsets.py
+-rw-rw-rw-   0        0        0     1471 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/wagtail_forms.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:33:08.703131 gdmty_django_users-24.5.0/src/gdmty_django_users.egg-info/
+-rw-rw-rw-   0        0        0    43714 2024-05-10 04:33:08.000000 gdmty_django_users-24.5.0/src/gdmty_django_users.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2024-05-10 04:33:08.000000 gdmty_django_users-24.5.0/src/gdmty_django_users.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 04:33:08.000000 gdmty_django_users-24.5.0/src/gdmty_django_users.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2024-05-10 04:33:08.000000 gdmty_django_users-24.5.0/src/gdmty_django_users.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-10 04:33:08.000000 gdmty_django_users-24.5.0/src/gdmty_django_users.egg-info/top_level.txt
```

### Comparing `gdmty_django_users-24.4.2/LICENSE` & `gdmty_django_users-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.4.2/PKG-INFO` & `gdmty_django_users-24.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gdmty-django-users
-Version: 24.4.2
-Summary: Custom Django Rest Framework authentication backend based on email and password for users in Administration panel with reCaptcha token verification.
+Version: 24.5.0
+Summary: Extension of Django's AbstractBaseUser for user management, using email as user.
 Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -660,16 +660,16 @@
         solutions will be better for different programs; see section 13 for the
         specific requirements.
         
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
-Project-URL: Homepage, https://github.com/gobiernodigital/gdmty-django-users
-Project-URL: Bug Tracker, https://github.com/gobiernodigital/gdmty-django-users/issues
+Project-URL: Homepage, https://github.com/gobiernodigitalmonterrey/gdmty-django-users
+Project-URL: Bug Tracker, https://github.com/gobiernodigitalmonterrey/gdmty-django-users/issues
 Keywords: django,recaptcha,users
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4
 Requires-Python: >=3.9
@@ -683,15 +683,15 @@
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # gdmty-django-users
 
-It's an django app named `gdmty-django-users` of users implemetation that extends AbstractBaseUser for use e-mail as user. And has the option to authenticate with reCaptcha token verification.
+The app `gdmty-django-users` package is a Django extension that builds upon the abstract AbstractBaseUser class for use e-mail as user. And has the option to authenticate with reCaptcha token verification.
 
 The project is maintained by Gobierno de Monterrey. You can find more about the project on
 its [homepage](https://github.com/gobiernodigitalmonterrey/gdmty-django-users) or report issues on
 the [bug tracker](https://github.com/gobiernodigitalmonterrey/gdmty-django-users/issues).
 
 ## Features
```

### Comparing `gdmty_django_users-24.4.2/README.md` & `gdmty_django_users-24.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # gdmty-django-users
 
-It's an django app named `gdmty-django-users` of users implemetation that extends AbstractBaseUser for use e-mail as user. And has the option to authenticate with reCaptcha token verification.
+The app `gdmty-django-users` package is a Django extension that builds upon the abstract AbstractBaseUser class for use e-mail as user. And has the option to authenticate with reCaptcha token verification.
 
 The project is maintained by Gobierno de Monterrey. You can find more about the project on
 its [homepage](https://github.com/gobiernodigitalmonterrey/gdmty-django-users) or report issues on
 the [bug tracker](https://github.com/gobiernodigitalmonterrey/gdmty-django-users/issues).
 
 ## Features
```

### Comparing `gdmty_django_users-24.4.2/pyproject.toml` & `gdmty_django_users-24.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gdmty-django-users"
-version = "24.4.2"
-description = "Custom Django Rest Framework authentication backend based on email and password for users in Administration panel with reCaptcha token verification."
+version = "24.5.0"
+description = "Extension of Django's AbstractBaseUser for user management, using email as user."
 readme = "README.md"
 authors = [{ name="Gobierno de Monterrey", email="cesar.benjamin@monterrey.gob.mx" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -27,19 +27,19 @@
 
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
-"Homepage" = "https://github.com/gobiernodigital/gdmty-django-users"
-"Bug Tracker" = "https://github.com/gobiernodigital/gdmty-django-users/issues"
+"Homepage" = "https://github.com/gobiernodigitalmonterrey/gdmty-django-users"
+"Bug Tracker" = "https://github.com/gobiernodigitalmonterrey/gdmty-django-users/issues"
 
 [tool.bumpver]
-current_version = "24.4.2"
+current_version = "24.5.0"
 version_pattern = "MAJOR.MINOR.PATCH[-PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `gdmty_django_users-24.4.2/src/gdmty_django_users/__init__.py` & `gdmty_django_users-24.5.0/src/gdmty_django_users/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!-*- coding: utf-8 -*-
 """
-Authentication backend for Django's Administration panel users based on email and password
+Package that is an extension of Django's AbstractBaseUser for user management, using email as user.
 This packages adds features such as group permissions and reCaptcha enterprise token verification.
 
 This package is published as free software under the terms of the Apache License, Version 2.0. Is developed by
 Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
-<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
+<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <cdgva@outlook.com>']
 Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-django-users
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 
 """
 
 __title__ = "gdmty_django_users"
-__version__ = "24.4.2"
+__version__ = "24.5.0"
 __description__ = "Django module for Users models and permission adding reCAPTCHA token verification."
 __url__ = "https://github.com/SIGAMty/gdmty-django-recaptcha-enterprise"
 __author__ = "César Benjamín"
 __author_email__ = "mathereall@gmail.com"
 __license__ = "GNU Affero General Public License v3 or later (AGPLv3+)"
 __keywords__ = ["django", "users"]
 VERSION = __version__
```

### Comparing `gdmty_django_users-24.4.2/src/gdmty_django_users/admin.py` & `gdmty_django_users-24.5.0/src/gdmty_django_users/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!-*- coding: utf-8 -*-
 """
-Authentication backend for Django's Administration panel users based on email and password
+Package that is an extension of Django's AbstractBaseUser for user management, using email as user.
 This packages adds features such as group permissions and reCaptcha enterprise token verification.
 
 This package is published as free software under the terms of the Apache License, Version 2.0. Is developed by
 Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
-<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
+<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <cdgva@outlook.com>']
 Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-django-users
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: AGPL-3.0
 
 """
 
 from django.contrib import admin
```

### Comparing `gdmty_django_users-24.4.2/src/gdmty_django_users/apps.py` & `gdmty_django_users-24.5.0/src/gdmty_django_users/apps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!-*- coding: utf-8 -*-
 """
-Authentication backend for Django's Administration panel users based on email and password
+Package that is an extension of Django's AbstractBaseUser for user management, using email as user.
 This packages adds features such as group permissions and reCaptcha enterprise token verification.
 
 This package is published as free software under the terms of the Apache License, Version 2.0. Is developed by
 Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
-<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
+<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <cdgva@outlook.com>']
 Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-django-users
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: AGPL-3.0
 
 """
 
 from django.apps import AppConfig
```

### Comparing `gdmty_django_users-24.4.2/src/gdmty_django_users/decorators.py` & `gdmty_django_users-24.5.0/src/gdmty_django_users/decorators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!-*- coding: utf-8 -*-
 """
-Authentication backend for Django's Administration panel users based on email and password
+Package that is an extension of Django's AbstractBaseUser for user management, using email as user.
 This packages adds features such as group permissions and reCaptcha enterprise token verification.
 
 This package is published as free software under the terms of the Apache License, Version 2.0. Is developed by
 Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
-<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
+<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <cdgva@outlook.com>']
 Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-django-users
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: AGPL-3.0
 """
 
 from functools import wraps
 from gdmty_django_recaptcha_enterprise.decorators import requires_recaptcha_token
```

### Comparing `gdmty_django_users-24.4.2/src/gdmty_django_users/managers.py` & `gdmty_django_users-24.5.0/src/gdmty_django_users/managers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!-*- coding: utf-8 -*-
 """
-Authentication backend for Django's Administration panel users based on email and password
+Package that is an extension of Django's AbstractBaseUser for user management, using email as user.
 This packages adds features such as group permissions and reCaptcha enterprise token verification.
 
 This package is published as free software under the terms of the Apache License, Version 2.0. Is developed by
 Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
-<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
+<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <cdgva@outlook.com>']
 Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-django-users
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: AGPL-3.0
 """
 
 from django.contrib.auth.base_user import BaseUserManager
 from django.utils.translation import gettext_lazy as _
```

### Comparing `gdmty_django_users-24.4.2/src/gdmty_django_users/migrations/0001_initial.py` & `gdmty_django_users-24.5.0/src/gdmty_django_users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.4.2/src/gdmty_django_users/models.py` & `gdmty_django_users-24.5.0/src/gdmty_django_users/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!-*- coding: utf-8 -*-
 """
-Authentication backend for Django's Administration panel users based on email and password
+Package that is an extension of Django's AbstractBaseUser for user management, using email as user.
 This packages adds features such as group permissions and reCaptcha enterprise token verification.
 
 This package is published as free software under the terms of the Apache License, Version 2.0. Is developed by
 Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
-<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
+<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <cdgva@outlook.com>']
 Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-django-users
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: AGPL-3.0
 """
 
 from django.db import models
 from django.contrib.auth.models import AbstractUser
```

### Comparing `gdmty_django_users-24.4.2/src/gdmty_django_users/permissions.py` & `gdmty_django_users-24.5.0/src/gdmty_django_users/permissions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!-*- coding: utf-8 -*-
 """
-Authentication backend for Django's Administration panel users based on email and password
+Package that is an extension of Django's AbstractBaseUser for user management, using email as user.
 This packages adds features such as group permissions and reCaptcha enterprise token verification.
 
 This package is published as free software under the terms of the Apache License, Version 2.0. Is developed by
 Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
-<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
+<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <cdgva@outlook.com>']
 Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-django-users
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: AGPL-3.0
 """
 
 from rest_framework import permissions
 from rest_framework.permissions import SAFE_METHODS
```

### Comparing `gdmty_django_users-24.4.2/src/gdmty_django_users/serializers.py` & `gdmty_django_users-24.5.0/src/gdmty_django_users/serializers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!-*- coding: utf-8 -*-
 """
-Authentication backend for Django's Administration panel users based on email and password
+Package that is an extension of Django's AbstractBaseUser for user management, using email as user.
 This packages adds features such as group permissions and reCaptcha enterprise token verification.
 
 This package is published as free software under the terms of the Apache License, Version 2.0. Is developed by
 Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
-<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
+<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <cdgva@outlook.com>']
 Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-django-users
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: AGPL-3.0
 """
 
 from rest_framework import serializers
 from .models import User, Group
```

### Comparing `gdmty_django_users-24.4.2/src/gdmty_django_users/settings.py` & `gdmty_django_users-24.5.0/src/gdmty_django_users/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!-*- coding: utf-8 -*-
 """
-Authentication backend for Django's Administration panel users based on email and password
+Package that is an extension of Django's AbstractBaseUser for user management, using email as user.
 This packages adds features such as group permissions and reCaptcha enterprise token verification.
 
 This package is published as free software under the terms of the Apache License, Version 2.0. Is developed by
 Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
-<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
+<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <cdgva@outlook.com>']
 Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-django-users
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: AGPL-3.0
 """
 
 import os
 from django.conf import settings
```

### Comparing `gdmty_django_users-24.4.2/src/gdmty_django_users/urls.py` & `gdmty_django_users-24.5.0/src/gdmty_django_users/urls.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!-*- coding: utf-8 -*-
 """
-Authentication backend for Django's Administration panel users based on email and password
+Package that is an extension of Django's AbstractBaseUser for user management, using email as user.
 This packages adds features such as group permissions and reCaptcha enterprise token verification.
 
 This package is published as free software under the terms of the Apache License, Version 2.0. Is developed by
 Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
-<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
+<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <cdgva@outlook.com>']
 Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-django-users
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: AGPL-3.0
 """
 
 from django.urls import path, include
 from .viewsets import UserViewSet, GroupViewSet, PermissionViewSet
```

### Comparing `gdmty_django_users-24.4.2/src/gdmty_django_users/viewsets.py` & `gdmty_django_users-24.5.0/src/gdmty_django_users/viewsets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!-*- coding: utf-8 -*-
 """
-Authentication backend for Django's Administration panel users based on email and password
+Package that is an extension of Django's AbstractBaseUser for user management, using email as user.
 This packages adds features such as group permissions and reCaptcha enterprise token verification.
 
 This package is published as free software under the terms of the Apache License, Version 2.0. Is developed by
 Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
-<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
+<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <cdgva@outlook.com>']
 Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-django-users
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: AGPL-3.0
 """
 
 from rest_framework import viewsets
 from .models import User, Group
```

### Comparing `gdmty_django_users-24.4.2/src/gdmty_django_users/wagtail_forms.py` & `gdmty_django_users-24.5.0/src/gdmty_django_users/wagtail_forms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!-*- coding: utf-8 -*-
 """
-Authentication backend for Django's Administration panel users based on email and password
+Package that is an extension of Django's AbstractBaseUser for user management, using email as user.
 This packages adds features such as group permissions and reCaptcha enterprise token verification.
 
 This package is published as free software under the terms of the Apache License, Version 2.0. Is developed by
 Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
-<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
+<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <cdgva@outlook.com>']
 Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-django-users
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: AGPL-3.0
 """
 
 from django import forms
 from django.utils.translation import gettext_lazy as _
```

### Comparing `gdmty_django_users-24.4.2/src/gdmty_django_users.egg-info/PKG-INFO` & `gdmty_django_users-24.5.0/src/gdmty_django_users.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gdmty-django-users
-Version: 24.4.2
-Summary: Custom Django Rest Framework authentication backend based on email and password for users in Administration panel with reCaptcha token verification.
+Version: 24.5.0
+Summary: Extension of Django's AbstractBaseUser for user management, using email as user.
 Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -660,16 +660,16 @@
         solutions will be better for different programs; see section 13 for the
         specific requirements.
         
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
-Project-URL: Homepage, https://github.com/gobiernodigital/gdmty-django-users
-Project-URL: Bug Tracker, https://github.com/gobiernodigital/gdmty-django-users/issues
+Project-URL: Homepage, https://github.com/gobiernodigitalmonterrey/gdmty-django-users
+Project-URL: Bug Tracker, https://github.com/gobiernodigitalmonterrey/gdmty-django-users/issues
 Keywords: django,recaptcha,users
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4
 Requires-Python: >=3.9
@@ -683,15 +683,15 @@
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # gdmty-django-users
 
-It's an django app named `gdmty-django-users` of users implemetation that extends AbstractBaseUser for use e-mail as user. And has the option to authenticate with reCaptcha token verification.
+The app `gdmty-django-users` package is a Django extension that builds upon the abstract AbstractBaseUser class for use e-mail as user. And has the option to authenticate with reCaptcha token verification.
 
 The project is maintained by Gobierno de Monterrey. You can find more about the project on
 its [homepage](https://github.com/gobiernodigitalmonterrey/gdmty-django-users) or report issues on
 the [bug tracker](https://github.com/gobiernodigitalmonterrey/gdmty-django-users/issues).
 
 ## Features
```

### Comparing `gdmty_django_users-24.4.2/src/gdmty_django_users.egg-info/SOURCES.txt` & `gdmty_django_users-24.5.0/src/gdmty_django_users.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 src/gdmty_django_users/wagtail_forms.py
 src/gdmty_django_users.egg-info/PKG-INFO
 src/gdmty_django_users.egg-info/SOURCES.txt
 src/gdmty_django_users.egg-info/dependency_links.txt
 src/gdmty_django_users.egg-info/requires.txt
 src/gdmty_django_users.egg-info/top_level.txt
 src/gdmty_django_users/migrations/0001_initial.py
+src/gdmty_django_users/migrations/0002_alter_user_groups_alter_user_user_permissions_and_more.py
 src/gdmty_django_users/migrations/__init__.py
```

