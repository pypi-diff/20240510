# Comparing `tmp/py4web-1.20240507.1.tar.gz` & `tmp/py4web-1.20240509.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20240507.1.tar", last modified: Wed May  8 05:54:16 2024, max compression
+gzip compressed data, was "py4web-1.20240509.1.tar", last modified: Fri May 10 05:27:06 2024, max compression
```

## Comparing `py4web-1.20240507.1.tar` & `py4web-1.20240509.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-08 05:54:16.814381 py4web-1.20240507.1/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20240507.1/LICENSE.md
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7746 2024-05-08 05:54:16.814381 py4web-1.20240507.1/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7174 2024-04-28 19:36:37.000000 py4web-1.20240507.1/README.rst
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-08 05:54:16.771046 py4web-1.20240507.1/py4web/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      764 2024-05-08 05:52:53.000000 py4web-1.20240507.1/py4web/__init__.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-08 05:54:16.797714 py4web-1.20240507.1/py4web/assets/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  2990688 2024-05-08 05:54:08.000000 py4web-1.20240507.1/py4web/assets/py4web.app._dashboard.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   187155 2024-05-08 05:54:08.000000 py4web-1.20240507.1/py4web/assets/py4web.app._default.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  4406167 2024-05-08 05:54:09.000000 py4web-1.20240507.1/py4web/assets/py4web.app._documentation.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5245 2024-05-08 05:54:08.000000 py4web-1.20240507.1/py4web/assets/py4web.app._minimal.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    21723 2024-05-08 05:54:08.000000 py4web-1.20240507.1/py4web/assets/py4web.app._scaffold.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  1392764 2024-05-08 05:54:09.000000 py4web-1.20240507.1/py4web/assets/py4web.app.showcase.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    68805 2024-05-08 05:51:19.000000 py4web-1.20240507.1/py4web/core.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    20383 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/server_adapters.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-08 05:54:16.804381 py4web-1.20240507.1/py4web/utils/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20240507.1/py4web/utils/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    72777 2024-05-08 05:42:38.000000 py4web-1.20240507.1/py4web/utils/auth.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-08 05:54:16.811048 py4web-1.20240507.1/py4web/utils/auth_plugins/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6440 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      797 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/basic_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1480 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/email_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35452 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/ldap_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2discord.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      670 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2facebook.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      474 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2github.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    11958 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2google_scoped.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2okta.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2079 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2server.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6091 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5082 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/pam.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/pam_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6620 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/saml2_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2811 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/auth_plugins/x509_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20240507.1/py4web/utils/cors.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1628 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/dbstore.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2046 2024-05-08 05:21:14.000000 py4web-1.20240507.1/py4web/utils/downloader.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3097 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/factories.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35921 2024-05-02 06:57:14.000000 py4web-1.20240507.1/py4web/utils/form.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69667 2024-05-02 06:57:02.000000 py4web-1.20240507.1/py4web/utils/grid.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1629 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/jsonrpc.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    34797 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/mailer.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9181 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/misc.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20240507.1/py4web/utils/param.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18284 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/populate.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1602 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/publisher.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2425 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/recaptcha.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3712 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/security.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      124 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6578 2024-04-28 19:36:37.000000 py4web-1.20240507.1/py4web/utils/url_signer.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-08 05:54:16.774379 py4web-1.20240507.1/py4web.egg-info/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7746 2024-05-08 05:54:16.000000 py4web-1.20240507.1/py4web.egg-info/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1896 2024-05-08 05:54:16.000000 py4web-1.20240507.1/py4web.egg-info/SOURCES.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-05-08 05:54:16.000000 py4web-1.20240507.1/py4web.egg-info/dependency_links.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       43 2024-05-08 05:54:16.000000 py4web-1.20240507.1/py4web.egg-info/entry_points.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      237 2024-05-08 05:54:16.000000 py4web-1.20240507.1/py4web.egg-info/requires.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        7 2024-05-08 05:54:16.000000 py4web-1.20240507.1/py4web.egg-info/top_level.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      843 2024-05-08 05:52:21.000000 py4web-1.20240507.1/pyproject.toml
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      462 2024-04-28 20:10:23.000000 py4web-1.20240507.1/requirements.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-05-08 05:54:16.814381 py4web-1.20240507.1/setup.cfg
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-08 05:54:16.814381 py4web-1.20240507.1/tests/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3462 2023-11-14 06:31:07.000000 py4web-1.20240507.1/tests/test_action.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8104 2024-04-28 20:10:23.000000 py4web-1.20240507.1/tests/test_auth.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_cache.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_fixture.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_form.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_get_error_snapshot.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_json.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_main.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_session.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20240507.1/tests/test_template.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      440 2024-04-07 06:47:57.000000 py4web-1.20240507.1/tests/test_url.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-10 05:27:06.565761 py4web-1.20240509.1/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20240509.1/LICENSE.md
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7746 2024-05-10 05:27:06.565761 py4web-1.20240509.1/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7174 2024-04-28 19:36:37.000000 py4web-1.20240509.1/README.rst
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-10 05:27:06.532426 py4web-1.20240509.1/py4web/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      764 2024-05-10 05:26:17.000000 py4web-1.20240509.1/py4web/__init__.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-10 05:27:06.552427 py4web-1.20240509.1/py4web/assets/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  2990688 2024-05-10 05:26:58.000000 py4web-1.20240509.1/py4web/assets/py4web.app._dashboard.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   187155 2024-05-10 05:26:58.000000 py4web-1.20240509.1/py4web/assets/py4web.app._default.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  4406167 2024-05-10 05:26:59.000000 py4web-1.20240509.1/py4web/assets/py4web.app._documentation.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5245 2024-05-10 05:26:58.000000 py4web-1.20240509.1/py4web/assets/py4web.app._minimal.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    21723 2024-05-10 05:26:58.000000 py4web-1.20240509.1/py4web/assets/py4web.app._scaffold.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  1392764 2024-05-10 05:26:59.000000 py4web-1.20240509.1/py4web/assets/py4web.app.showcase.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    68805 2024-05-10 05:25:35.000000 py4web-1.20240509.1/py4web/core.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    20383 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/server_adapters.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-10 05:27:06.559094 py4web-1.20240509.1/py4web/utils/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20240509.1/py4web/utils/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    72777 2024-05-08 05:42:38.000000 py4web-1.20240509.1/py4web/utils/auth.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-10 05:27:06.562427 py4web-1.20240509.1/py4web/utils/auth_plugins/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6440 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      797 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/basic_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1480 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/email_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35452 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/ldap_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2discord.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      670 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2facebook.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      474 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2github.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    11958 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2google_scoped.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2okta.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2079 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2server.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6091 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5082 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/pam.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/pam_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6620 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/saml2_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2811 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/auth_plugins/x509_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20240509.1/py4web/utils/cors.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1628 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/dbstore.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2046 2024-05-08 05:21:14.000000 py4web-1.20240509.1/py4web/utils/downloader.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3097 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/factories.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35921 2024-05-02 06:57:14.000000 py4web-1.20240509.1/py4web/utils/form.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69667 2024-05-02 06:57:02.000000 py4web-1.20240509.1/py4web/utils/grid.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1629 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/jsonrpc.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    34797 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/mailer.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9181 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/misc.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20240509.1/py4web/utils/param.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18284 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/populate.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1602 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/publisher.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2425 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/recaptcha.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3712 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/security.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      124 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6578 2024-04-28 19:36:37.000000 py4web-1.20240509.1/py4web/utils/url_signer.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-10 05:27:06.532426 py4web-1.20240509.1/py4web.egg-info/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7746 2024-05-10 05:27:06.000000 py4web-1.20240509.1/py4web.egg-info/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1896 2024-05-10 05:27:06.000000 py4web-1.20240509.1/py4web.egg-info/SOURCES.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-05-10 05:27:06.000000 py4web-1.20240509.1/py4web.egg-info/dependency_links.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       43 2024-05-10 05:27:06.000000 py4web-1.20240509.1/py4web.egg-info/entry_points.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      237 2024-05-10 05:27:06.000000 py4web-1.20240509.1/py4web.egg-info/requires.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        7 2024-05-10 05:27:06.000000 py4web-1.20240509.1/py4web.egg-info/top_level.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      843 2024-05-10 05:26:03.000000 py4web-1.20240509.1/pyproject.toml
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      462 2024-04-28 20:10:23.000000 py4web-1.20240509.1/requirements.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-05-10 05:27:06.565761 py4web-1.20240509.1/setup.cfg
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-10 05:27:06.565761 py4web-1.20240509.1/tests/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3462 2023-11-14 06:31:07.000000 py4web-1.20240509.1/tests/test_action.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8104 2024-04-28 20:10:23.000000 py4web-1.20240509.1/tests/test_auth.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_cache.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_fixture.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_form.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_get_error_snapshot.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_json.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_main.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_session.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20240509.1/tests/test_template.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      440 2024-04-07 06:47:57.000000 py4web-1.20240509.1/tests/test_url.py
```

### Comparing `py4web-1.20240507.1/LICENSE.md` & `py4web-1.20240509.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/PKG-INFO` & `py4web-1.20240509.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20240507.1
+Version: 1.20240509.1
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20240507.1/README.rst` & `py4web-1.20240509.1/README.rst`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/__init__.py` & `py4web-1.20240509.1/py4web/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 __author__ = "Massimo Di Pierro <massimo.dipierro@gmail.com>"
 __license__ = "BSD-3-Clause"
-__version__ = "1.20240507.1"
+__version__ = "1.20240509.1"
 
 
 def _maybe_gevent():
     for arg in sys.argv[1:]:
         if "gevent" in arg.lower():
             from gevent import monkey
```

### Comparing `py4web-1.20240507.1/py4web/assets/py4web.app._dashboard.zip` & `py4web-1.20240509.1/py4web/assets/py4web.app._dashboard.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/assets/py4web.app._default.zip` & `py4web-1.20240509.1/py4web/assets/py4web.app._default.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/assets/py4web.app._documentation.zip` & `py4web-1.20240509.1/py4web/assets/py4web.app._documentation.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/assets/py4web.app._minimal.zip` & `py4web-1.20240509.1/py4web/assets/py4web.app._minimal.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/assets/py4web.app._scaffold.zip` & `py4web-1.20240509.1/py4web/assets/py4web.app._scaffold.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/assets/py4web.app.showcase.zip` & `py4web-1.20240509.1/py4web/assets/py4web.app.showcase.zip`

 * *Files 0% similar despite different names*

#### zipinfo {}

```diff
@@ -1,38 +1,38 @@
 Zip file size: 1392764 bytes, number of entries: 143
 -rw-r--r--  3.0 unx       20 tx stor 23-May-08 00:39 uploads/README.md
--rw-r--r--  3.0 unx     4206 tx defN 24-Apr-28 19:36 __init__.py
+-rw-r--r--  3.0 unx     4206 tx defN 24-May-09 05:43 __init__.py
 -rw-r--r--  3.0 unx      349 tx defN 23-May-08 00:39 examples/count.py
 -rwxr--r--  3.0 unx      422 tx defN 23-May-08 00:39 examples/ws_client_example.py
 -rw-r--r--  3.0 unx       88 tx defN 23-May-08 00:39 examples/page_with_error.py
 -rw-r--r--  3.0 unx      112 tx defN 23-May-08 00:39 examples/page_with_raise.py
 -rw-r--r--  3.0 unx      145 tx defN 23-May-08 00:39 examples/hello_world_msg.py
 -rw-r--r--  3.0 unx      414 tx defN 23-May-08 00:39 examples/test_expose.py
 -rw-r--r--  3.0 unx      281 tx defN 23-May-08 00:39 examples/page_with_parameters.py
 -rw-r--r--  3.0 unx      125 tx defN 23-May-08 00:39 examples/hello_world.py
 -rw-r--r--  3.0 unx      227 tx defN 23-May-08 00:39 examples/page_with_query.py
 -rw-r--r--  3.0 unx     1583 tx defN 23-May-08 00:39 examples/example_html_grid.py
 -rw-r--r--  3.0 unx      181 tx defN 23-May-08 00:39 examples/page_with_redirect.py
 -rw-r--r--  3.0 unx      197 tx defN 23-May-08 00:39 examples/session_clear.py
--rw-r--r--  3.0 unx     2617 tx defN 23-May-08 00:39 examples/models.py
+-rw-r--r--  3.0 unx     2617 tx defN 24-May-09 05:54 examples/models.py
 -rw-r--r--  3.0 unx      372 tx defN 23-May-08 00:39 examples/flash_example_fixture.py
 -rw-r--r--  3.0 unx      396 tx defN 23-May-08 00:39 examples/custom_form.py
 -rw-r--r--  3.0 unx      644 tx defN 23-May-08 00:39 examples/rpc.py
 -rw-r--r--  3.0 unx      264 tx defN 23-May-08 00:39 examples/session_counter.py
 -rw-r--r--  3.0 unx      517 tx defN 23-May-08 00:39 examples/socketio.py
 -rw-r--r--  3.0 unx      647 tx defN 23-May-08 00:39 examples/auth_forms.py
 -rw-r--r--  3.0 unx     2749 tx defN 23-May-08 00:39 examples/rest.py
--rw-r--r--  3.0 unx     4809 tx defN 23-May-08 00:39 examples/common.py
+-rw-r--r--  3.0 unx     4809 tx defN 24-May-09 05:51 examples/common.py
 -rw-r--r--  3.0 unx      171 tx defN 23-May-08 00:39 examples/page_with_template.py
 -rw-r--r--  3.0 unx      378 tx defN 23-May-08 00:39 examples/auth_form.py
 -rw-r--r--  3.0 unx      456 tx defN 23-May-08 00:39 examples/create_form.py
 -rw-r--r--  3.0 unx      272 tx defN 23-May-08 00:39 examples/ws.py
 -rw-r--r--  3.0 unx      255 tx defN 23-May-08 00:39 examples/show_a_button.py
 -rw-r--r--  3.0 unx      106 tx defN 23-May-08 00:39 examples/page_without_template.py
--rw-r--r--  3.0 unx     1467 tx defN 24-May-08 05:06 examples/settings.py
+-rw-r--r--  3.0 unx     1467 tx defN 24-May-09 05:56 examples/settings.py
 -rw-r--r--  3.0 unx      420 tx defN 23-May-08 00:39 examples/page_with_postback.py
 -rw-r--r--  3.0 unx      465 tx defN 23-May-08 00:39 examples/update_form.py
 -rw-r--r--  3.0 unx     1966 tx defN 23-May-08 00:39 examples/example_multiple_forms.py
 -rw-r--r--  3.0 unx      870 tx defN 23-May-08 00:39 examples/component_loader.py
 -rw-r--r--  3.0 unx      130 tx defN 23-May-08 00:39 examples/hello.py
 -rw-r--r--  3.0 unx      375 tx defN 23-May-08 00:39 examples/tagsinput_form.py
 -rw-r--r--  3.0 unx      236 tx defN 23-May-08 00:39 examples/example_helpers.py
```

### Comparing `py4web-1.20240507.1/py4web/core.py` & `py4web-1.20240509.1/py4web/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -946,15 +946,15 @@
                 ret = func(*func_args, **func_kwargs)
                 if isinstance(ret, (list, dict)):
                     response.headers["Content-Type"] = "application/json"
                     ret = dumps(ret)
                 elif ret is None:
                     ret = ""
                 elif isinstance(ret, yatl.helpers.TAGGER):
-                    res = str(ret)
+                    ret = str(ret)
                 elif not hasattr(ret, "__iter__"):
                     raise RuntimeError(f"Cannot return type {ret.__class__.__name__}")
                 return ret
             except HTTP as http:
                 response.status = http.status
                 response.headers.update(http.headers)
                 body = http.body
```

### Comparing `py4web-1.20240507.1/py4web/server_adapters.py` & `py4web-1.20240509.1/py4web/server_adapters.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/auth.py` & `py4web-1.20240509.1/py4web/utils/auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/auth_plugins/__init__.py` & `py4web-1.20240509.1/py4web/utils/auth_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/auth_plugins/basic_auth_plugin.py` & `py4web-1.20240509.1/py4web/utils/auth_plugins/basic_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/auth_plugins/email_auth_plugin.py` & `py4web-1.20240509.1/py4web/utils/auth_plugins/email_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/auth_plugins/ldap_plugin.py` & `py4web-1.20240509.1/py4web/utils/auth_plugins/ldap_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2discord.py` & `py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2discord.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2facebook.py` & `py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2facebook.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2google.py` & `py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2google.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2google_scoped.py` & `py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2google_scoped.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2server.py` & `py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2server.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/auth_plugins/oauth2wpminiorange.py` & `py4web-1.20240509.1/py4web/utils/auth_plugins/oauth2wpminiorange.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/auth_plugins/pam.py` & `py4web-1.20240509.1/py4web/utils/auth_plugins/pam.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/auth_plugins/saml2_plugin.py` & `py4web-1.20240509.1/py4web/utils/auth_plugins/saml2_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/auth_plugins/x509_auth_plugin.py` & `py4web-1.20240509.1/py4web/utils/auth_plugins/x509_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/cors.py` & `py4web-1.20240509.1/py4web/utils/cors.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/dbstore.py` & `py4web-1.20240509.1/py4web/utils/dbstore.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/downloader.py` & `py4web-1.20240509.1/py4web/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/factories.py` & `py4web-1.20240509.1/py4web/utils/factories.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/form.py` & `py4web-1.20240509.1/py4web/utils/form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/grid.py` & `py4web-1.20240509.1/py4web/utils/grid.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/jsonrpc.py` & `py4web-1.20240509.1/py4web/utils/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/mailer.py` & `py4web-1.20240509.1/py4web/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/misc.py` & `py4web-1.20240509.1/py4web/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/populate.py` & `py4web-1.20240509.1/py4web/utils/populate.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/publisher.py` & `py4web-1.20240509.1/py4web/utils/publisher.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/recaptcha.py` & `py4web-1.20240509.1/py4web/utils/recaptcha.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/security.py` & `py4web-1.20240509.1/py4web/utils/security.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web/utils/url_signer.py` & `py4web-1.20240509.1/py4web/utils/url_signer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/py4web.egg-info/PKG-INFO` & `py4web-1.20240509.1/py4web.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20240507.1
+Version: 1.20240509.1
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20240507.1/py4web.egg-info/SOURCES.txt` & `py4web-1.20240509.1/py4web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/pyproject.toml` & `py4web-1.20240509.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "py4web"
-version = "1.20240507.1"
+version = "1.20240509.1"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = "A fast, stable, comprehensive web framework"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
```

### Comparing `py4web-1.20240507.1/tests/test_action.py` & `py4web-1.20240509.1/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/tests/test_auth.py` & `py4web-1.20240509.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/tests/test_cache.py` & `py4web-1.20240509.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/tests/test_fixture.py` & `py4web-1.20240509.1/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/tests/test_form.py` & `py4web-1.20240509.1/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/tests/test_get_error_snapshot.py` & `py4web-1.20240509.1/tests/test_get_error_snapshot.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/tests/test_json.py` & `py4web-1.20240509.1/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/tests/test_main.py` & `py4web-1.20240509.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/tests/test_session.py` & `py4web-1.20240509.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240507.1/tests/test_tags.py` & `py4web-1.20240509.1/tests/test_tags.py`

 * *Files identical despite different names*

