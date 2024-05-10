# Comparing `tmp/ccs-digitalmarketplace-utils-66.0.0rc3.tar.gz` & `tmp/ccs-digitalmarketplace-utils-66.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-utils-66.0.0rc3.tar", last modified: Thu May  9 14:00:09 2024, max compression
+gzip compressed data, was "ccs-digitalmarketplace-utils-66.0.0rc4.tar", last modified: Fri May 10 15:44:17 2024, max compression
```

## Comparing `ccs-digitalmarketplace-utils-66.0.0rc3.tar` & `ccs-digitalmarketplace-utils-66.0.0rc4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:09.677497 ccs-digitalmarketplace-utils-66.0.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-09 14:00:09.677497 ccs-digitalmarketplace-utils-66.0.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:09.669497 ccs-digitalmarketplace-utils-66.0.0rc3/ccs_digitalmarketplace_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-09 14:00:09.000000 ccs-digitalmarketplace-utils-66.0.0rc3/ccs_digitalmarketplace_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-09 14:00:09.000000 ccs-digitalmarketplace-utils-66.0.0rc3/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:00:09.000000 ccs-digitalmarketplace-utils-66.0.0rc3/ccs_digitalmarketplace_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-09 14:00:09.000000 ccs-digitalmarketplace-utils-66.0.0rc3/ccs_digitalmarketplace_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 14:00:09.000000 ccs-digitalmarketplace-utils-66.0.0rc3/ccs_digitalmarketplace_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:09.673497 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/asset_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/cloudfoundry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/compliance_communications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/cookie_probe.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/csv_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/direct_plus_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/dmp_so_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/documents.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:09.673497 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/email/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10873 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/email/dm_mailchimp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/email/dm_notify.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/email/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/email/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/email/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/email/user_account_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/env_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:09.673497 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/errors/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/errors/frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/external.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/flask_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:09.677497 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/forms/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/forms/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/forms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/forms/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/forms/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/jinja2_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/ods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:09.677497 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/presenters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/presenters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7286 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/presenters/compliance_communications.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/presenters/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/proxy_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:09.677497 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/repoutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/repoutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/request_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/service_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:00:09.677497 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/view_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/view_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/view_helpers/compliance_communications.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/view_helpers/frameworks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/view_helpers/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:00:09.677497 ccs-digitalmarketplace-utils-66.0.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-09 13:59:59.000000 ccs-digitalmarketplace-utils-66.0.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:44:17.515854 ccs-digitalmarketplace-utils-66.0.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-10 15:44:17.515854 ccs-digitalmarketplace-utils-66.0.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:44:17.503854 ccs-digitalmarketplace-utils-66.0.0rc4/ccs_digitalmarketplace_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-10 15:44:17.000000 ccs-digitalmarketplace-utils-66.0.0rc4/ccs_digitalmarketplace_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-10 15:44:17.000000 ccs-digitalmarketplace-utils-66.0.0rc4/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:44:17.000000 ccs-digitalmarketplace-utils-66.0.0rc4/ccs_digitalmarketplace_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-10 15:44:17.000000 ccs-digitalmarketplace-utils-66.0.0rc4/ccs_digitalmarketplace_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 15:44:17.000000 ccs-digitalmarketplace-utils-66.0.0rc4/ccs_digitalmarketplace_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:44:17.511854 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/asset_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/cloudfoundry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/compliance_communications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/cookie_probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/csv_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/direct_plus_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/dmp_so_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/documents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:44:17.511854 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/email/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10873 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/email/dm_mailchimp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/email/dm_notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/email/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/email/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/email/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/email/user_account_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/env_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:44:17.511854 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/errors/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/errors/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/flask_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:44:17.511854 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/forms/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/forms/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/forms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/forms/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/forms/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/jinja2_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/ods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:44:17.511854 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/presenters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/presenters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7286 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/presenters/compliance_communications.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/presenters/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/proxy_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:44:17.515854 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/repoutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/repoutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/request_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/service_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:44:17.515854 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/view_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/view_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/view_helpers/compliance_communications.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/view_helpers/frameworks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/view_helpers/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:44:17.515854 ccs-digitalmarketplace-utils-66.0.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-10 15:44:08.000000 ccs-digitalmarketplace-utils-66.0.0rc4/setup.py
```

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/LICENCE` & `ccs-digitalmarketplace-utils-66.0.0rc4/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/README.md` & `ccs-digitalmarketplace-utils-66.0.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt` & `ccs-digitalmarketplace-utils-66.0.0rc4/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/access_control.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/access_control.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from flask_login import current_user, login_required
-from flask import current_app, flash, Markup
+from flask import current_app, flash
+from markupsafe import Markup
 
 
 ROLES = {
     'buyer': {
         'loginRequiredMessage': Markup("You must log in with a buyer account to see this page."),
     },
     'supplier': {
```

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/asset_fingerprint.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/asset_fingerprint.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/authentication.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/authentication.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/cloudfoundry.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/cloudfoundry.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/compliance_communications.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/compliance_communications.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/config.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/config.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/cookie_probe.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/cookie_probe.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/csv_generator.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/csv_generator.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/dates.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/dates.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/deprecation.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/deprecation.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/direct_plus_client.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/direct_plus_client.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/documents.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/documents.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/email/dm_mailchimp.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/email/dm_mailchimp.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/email/dm_notify.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/email/dm_notify.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/email/helpers.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/email/helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/email/tokens.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/email/tokens.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/email/user_account_email.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/email/user_account_email.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/env_helpers.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/env_helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/errors/api.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/errors/api.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/errors/frontend.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/errors/frontend.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/external.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/external.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/feature_flag.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/feature_flag.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/filters.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/filters.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/flask.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/flask.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/flask_init.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/flask_init.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/formats.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/formats.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/forms/errors.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/forms/errors.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/forms/fields.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/forms/fields.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/forms/helpers.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/forms/helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/forms/mixins.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/forms/mixins.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/forms/validators.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/forms/validators.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/forms/widgets.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/jinja2_environment.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/jinja2_environment.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/logging.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/logging.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/ods.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/ods.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/presenters/compliance_communications.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/presenters/compliance_communications.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/presenters/helpers.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/presenters/helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/proxy_fix.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/proxy_fix.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/request_id.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/request_id.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/s3.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/s3.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/service_attribute.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/service_attribute.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/session.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/session.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/status.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/status.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/timing.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/timing.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/urls.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/urls.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/user.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/user.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/view_helpers/compliance_communications.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/view_helpers/compliance_communications.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/view_helpers/pagination.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/view_helpers/pagination.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/dmutils/views.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/dmutils/views.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc3/setup.py` & `ccs-digitalmarketplace-utils-66.0.0rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     description='Common utils for Digital Marketplace apps.',
     long_description=__doc__,
     packages=find_packages(),
     package_data={'dmutils': ['py.typed']},
     include_package_data=True,
     install_requires=[
         'Flask-WTF>=1.2.1',
-        'Flask>=2.2,<2.3',
+        'Flask>=2.3,<3',
         'Flask-gzip>=0.2',
         'Flask-Login>=0.6.3',
         'Flask-Session<0.9.0,>=0.8.0',
         'boto3<2,>=1.7.83',
         'contextlib2>=21.6.0',
         'cryptography>=41.0.4',
         'ccs-digitalmarketplace-apiclient>=25.0.0',
@@ -39,12 +39,12 @@
         'redis>=5.0.1',
         'fleep<1.1,>=1.0.1',
         'notifications-python-client>=8.1.0,<9.0.0',
         'odfpy>=1.4.1',
         'python-json-logger>=2.0.7,<3.0.0',
         'pytz',
         'unicodecsv>=0.14.1',
-        'werkzeug>=2.2,<2.3',
+        'werkzeug>=2.3,<3',
         'workdays>=1.4',
     ],
     python_requires=">=3.9,<3.13",
 )
```

