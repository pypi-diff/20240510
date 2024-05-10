# Comparing `tmp/wagtail-birdsong-1.2.0.tar.gz` & `tmp/wagtail_birdsong-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-birdsong-1.2.0.tar", last modified: Tue Jan  9 22:52:04 2024, max compression
+gzip compressed data, was "wagtail_birdsong-2.0.0.tar", last modified: Fri May 10 06:30:06 2024, max compression
```

## Comparing `wagtail-birdsong-1.2.0.tar` & `wagtail_birdsong-2.0.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.437283 wagtail-birdsong-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1518 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8502 2024-01-09 22:52:04.436283 wagtail-birdsong-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7718 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.429283 wagtail-birdsong-1.2.0/birdsong/
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      213 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.429283 wagtail-birdsong-1.2.0/birdsong/backends/
--rw-rw-rw-   0 root         (0) root         (0)      452 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/backends/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2388 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/backends/smtp.py
--rw-rw-rw-   0 root         (0) root         (0)      543 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/blocks.py
--rw-rw-rw-   0 root         (0) root         (0)      222 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.431283 wagtail-birdsong-1.2.0/birdsong/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1778 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1280 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/migrations/0002_auto_20200603_0206.py
--rw-rw-rw-   0 root         (0) root         (0)      389 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/migrations/0003_drop_unique_constraint.py
--rw-rw-rw-   0 root         (0) root         (0)      729 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/migrations/0004_campaign_status.py
--rw-rw-rw-   0 root         (0) root         (0)      389 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/migrations/0005_alter_receipt_success.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/migrations/0006_auto_20220428_0558.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/migrations/0007_alter_contacttag_tag.py
--rw-rw-rw-   0 root         (0) root         (0)     2130 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/migrations/0008_translation_support.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2569 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/models.py
--rw-rw-rw-   0 root         (0) root         (0)     6841 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.424283 wagtail-birdsong-1.2.0/birdsong/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.424283 wagtail-birdsong-1.2.0/birdsong/static/birdsong/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.431283 wagtail-birdsong-1.2.0/birdsong/static/birdsong/css/
--rw-rw-rw-   0 root         (0) root         (0)      457 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/static/birdsong/css/campaign-editor.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.432283 wagtail-birdsong-1.2.0/birdsong/static/birdsong/js/
--rw-rw-rw-   0 root         (0) root         (0)     2174 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/static/birdsong/js/preview_campaign.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.432283 wagtail-birdsong-1.2.0/birdsong/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.425283 wagtail-birdsong-1.2.0/birdsong/templates/birdsong/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.433283 wagtail-birdsong-1.2.0/birdsong/templates/birdsong/editor/
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/templates/birdsong/editor/create_campaign.html
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/templates/birdsong/editor/edit_campaign.html
--rw-rw-rw-   0 root         (0) root         (0)     1638 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/templates/birdsong/editor/inspect_campaign.html
--rw-rw-rw-   0 root         (0) root         (0)     1421 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/templates/birdsong/editor/send_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)     1080 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/templates/birdsong/editor/test_confirm.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.433283 wagtail-birdsong-1.2.0/birdsong/templates/birdsong/mail/
--rw-rw-rw-   0 root         (0) root         (0)      252 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/templates/birdsong/mail/base_email.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.433283 wagtail-birdsong-1.2.0/birdsong/templates/birdsong/mail/blocks/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/templates/birdsong/mail/blocks/richtext.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.434283 wagtail-birdsong-1.2.0/birdsong/templates/icons/
--rw-rw-rw-   0 root         (0) root         (0)      439 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/templates/icons/birdsong.svg
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/templates/unsubscribe.html
--rw-rw-rw-   0 root         (0) root         (0)      193 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.434283 wagtail-birdsong-1.2.0/birdsong/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1021 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/views/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     2934 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/views/editor.py
--rw-rw-rw-   0 root         (0) root         (0)      564 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/views/unsubscribe.py
--rw-rw-rw-   0 root         (0) root         (0)     3379 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/birdsong/wagtail_hooks.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-09 22:52:04.437283 wagtail-birdsong-1.2.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1261 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.435283 wagtail-birdsong-1.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3570 2024-01-09 22:51:56.000000 wagtail-birdsong-1.2.0/tests/test_admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-09 22:52:04.436283 wagtail-birdsong-1.2.0/wagtail_birdsong.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8502 2024-01-09 22:52:04.000000 wagtail-birdsong-1.2.0/wagtail_birdsong.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1606 2024-01-09 22:52:04.000000 wagtail-birdsong-1.2.0/wagtail_birdsong.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-09 22:52:04.000000 wagtail-birdsong-1.2.0/wagtail_birdsong.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-09 22:52:04.000000 wagtail-birdsong-1.2.0/wagtail_birdsong.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2024-01-09 22:52:04.000000 wagtail-birdsong-1.2.0/wagtail_birdsong.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-01-09 22:52:04.000000 wagtail-birdsong-1.2.0/wagtail_birdsong.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.790670 wagtail_birdsong-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8528 2024-05-10 06:30:06.790670 wagtail_birdsong-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7710 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.783671 wagtail_birdsong-2.0.0/birdsong/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      213 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.783671 wagtail_birdsong-2.0.0/birdsong/backends/
+-rw-rw-rw-   0 root         (0) root         (0)      452 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/backends/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2804 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/backends/smtp.py
+-rw-rw-rw-   0 root         (0) root         (0)      543 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.785670 wagtail_birdsong-2.0.0/birdsong/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1778 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1280 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/migrations/0002_auto_20200603_0206.py
+-rw-rw-rw-   0 root         (0) root         (0)      389 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/migrations/0003_drop_unique_constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)      729 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/migrations/0004_campaign_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      389 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/migrations/0005_alter_receipt_success.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/migrations/0006_auto_20220428_0558.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/migrations/0007_alter_contacttag_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/migrations/0008_translation_support.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2726 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6825 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.778671 wagtail_birdsong-2.0.0/birdsong/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.778671 wagtail_birdsong-2.0.0/birdsong/static/birdsong/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.785670 wagtail_birdsong-2.0.0/birdsong/static/birdsong/css/
+-rw-rw-rw-   0 root         (0) root         (0)      457 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/static/birdsong/css/campaign-editor.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.785670 wagtail_birdsong-2.0.0/birdsong/static/birdsong/js/
+-rw-rw-rw-   0 root         (0) root         (0)     2174 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/static/birdsong/js/preview_campaign.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.786671 wagtail_birdsong-2.0.0/birdsong/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.779671 wagtail_birdsong-2.0.0/birdsong/templates/birdsong/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.787670 wagtail_birdsong-2.0.0/birdsong/templates/birdsong/editor/
+-rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/templates/birdsong/editor/create_campaign.html
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/templates/birdsong/editor/edit_campaign.html
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/templates/birdsong/editor/inspect_campaign.html
+-rw-rw-rw-   0 root         (0) root         (0)     1421 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/templates/birdsong/editor/send_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/templates/birdsong/editor/test_confirm.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.787670 wagtail_birdsong-2.0.0/birdsong/templates/birdsong/mail/
+-rw-rw-rw-   0 root         (0) root         (0)      252 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/templates/birdsong/mail/base_email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.787670 wagtail_birdsong-2.0.0/birdsong/templates/birdsong/mail/blocks/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/templates/birdsong/mail/blocks/richtext.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.787670 wagtail_birdsong-2.0.0/birdsong/templates/icons/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/templates/icons/birdsong.svg
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/templates/unsubscribe.html
+-rw-rw-rw-   0 root         (0) root         (0)      193 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.788670 wagtail_birdsong-2.0.0/birdsong/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/views/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2926 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/views/editor.py
+-rw-rw-rw-   0 root         (0) root         (0)      564 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/views/unsubscribe.py
+-rw-rw-rw-   0 root         (0) root         (0)     3347 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/birdsong/wagtail_hooks.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 06:30:06.791670 wagtail_birdsong-2.0.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1291 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.788670 wagtail_birdsong-2.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3580 2024-05-10 06:29:57.000000 wagtail_birdsong-2.0.0/tests/test_admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 06:30:06.790670 wagtail_birdsong-2.0.0/wagtail_birdsong.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8528 2024-05-10 06:30:06.000000 wagtail_birdsong-2.0.0/wagtail_birdsong.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1606 2024-05-10 06:30:06.000000 wagtail_birdsong-2.0.0/wagtail_birdsong.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 06:30:06.000000 wagtail_birdsong-2.0.0/wagtail_birdsong.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 06:30:06.000000 wagtail_birdsong-2.0.0/wagtail_birdsong.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-10 06:30:06.000000 wagtail_birdsong-2.0.0/wagtail_birdsong.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-10 06:30:06.000000 wagtail_birdsong-2.0.0/wagtail_birdsong.egg-info/top_level.txt
```

### Comparing `wagtail-birdsong-1.2.0/LICENSE` & `wagtail_birdsong-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-birdsong-1.2.0/PKG-INFO` & `wagtail_birdsong-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-birdsong
-Version: 1.2.0
+Version: 2.0.0
 Summary: Create and send email campaigns from Wagtail
 Author: Neon Jungle
 Author-email: developers@neonjungle.studio
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,16 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: BSD License
 License-File: LICENSE
-Requires-Dist: wagtail>=4.1
+Requires-Dist: wagtail>=5.2
+Requires-Dist: wagtail-modeladmin
 Requires-Dist: django-mjml
 
 .. image:: docs/birdsong.svg
     :width: 400
     :alt: Birdsong Logo
 
 A plugin for wagtail that allows you to create, send, preview, edit and test email campaigns from within Wagtail.
@@ -47,15 +48,15 @@
 
 .. code-block:: python
 
     INSTALLED_APPS = [
         ...
         'mjml',
         'birdsong',
-        'wagtail.contrib.modeladmin',
+        'wagtail_modeladmin',
         ...
     ]
 
 Make a new app e.g. ``email``, create a ``models.py`` with a model that extends the included ``Campaign`` model. Some compatible mjml streamfield blocks are included in birdsong for convenience.
 
 ``models.py``
```

### Comparing `wagtail-birdsong-1.2.0/README.rst` & `wagtail_birdsong-2.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 .. code-block:: python
 
     INSTALLED_APPS = [
         ...
         'mjml',
         'birdsong',
-        'wagtail.contrib.modeladmin',
+        'wagtail_modeladmin',
         ...
     ]
 
 Make a new app e.g. ``email``, create a ``models.py`` with a model that extends the included ``Campaign`` model. Some compatible mjml streamfield blocks are included in birdsong for convenience.
 
 ``models.py``
```

### Comparing `wagtail-birdsong-1.2.0/birdsong/backends/smtp.py` & `wagtail_birdsong-2.0.0/birdsong/backends/smtp.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from smtplib import SMTPException
 from threading import Thread
 
 from django.db import close_old_connections, transaction
+from django.template.exceptions import TemplateDoesNotExist
 from django.template.loader import render_to_string
 from django.utils import timezone
 
 from birdsong.models import Campaign, CampaignStatus, Contact
 from birdsong.utils import send_mass_html_mail
 
 from . import BaseEmailBackend
@@ -18,50 +19,59 @@
     def __init__(self, campaign_pk, contact_pks, messages):
         super().__init__()
         self.campaign_pk = campaign_pk
         self.contact_pks = contact_pks
         self.messages = messages
 
     def run(self):
-        campaign_queryset = Campaign.objects.filter(pk=self.campaign_pk)
-        campaign = campaign_queryset.first()
+        campaign = Campaign.objects.get(pk=self.campaign_pk)
         try:
             logger.info(f"Sending {len(self.messages)} emails")
             send_mass_html_mail(self.messages)
             logger.info("Emails finished sending")
             with transaction.atomic():
-                campaign_queryset.update(
-                    status=CampaignStatus.SENT,
-                    sent_date=timezone.now(),
-                )
+                campaign.status = CampaignStatus.SENT
+                campaign.sent_date = timezone.now()
+                campaign.save()
                 fresh_contacts = Contact.objects.filter(pk__in=self.contact_pks)
                 campaign.receipts.add(*fresh_contacts)
         except SMTPException:
             logger.exception(f"Problem sending campaign: {self.campaign_pk}")
-            campaign_queryset.update(status=CampaignStatus.FAILED)
+            campaign.status = CampaignStatus.FAILED
+            campaign.save()
         finally:
             close_old_connections()
 
 
 class SMTPEmailBackend(BaseEmailBackend):
     def send_campaign(self, request, campaign, contacts, test_send=False):
         messages = []
 
         for contact in contacts:
-            content = render_to_string(
-                campaign.get_template(request),
-                campaign.get_context(request, contact),
-            )
-            messages.append({
+            message_data = {
                 'subject': campaign.subject,
-                'body': content,
                 'from_email': self.from_email,
                 'to': [contact.email],
                 'reply_to': [self.reply_to],
-            })
+
+            }
+            html_content = render_to_string(
+                campaign.get_template(request),
+                campaign.get_context(request, contact),
+            )
+            try:
+                text_content = render_to_string(
+                    campaign.get_text_template(request),
+                    campaign.get_context(request, contact),
+                )
+                message_data['body'] = text_content
+                message_data['html_body'] = html_content
+            except TemplateDoesNotExist:
+                message_data['body'] = html_content
+            messages.append(message_data)
         if test_send:
             # Don't mark as complete, don't worry about threading
             send_mass_html_mail(messages)
         else:
             campaign_thread = SendCampaignThread(
                 campaign.pk, [c.pk for c in contacts], messages)
             campaign_thread.start()
```

### Comparing `wagtail-birdsong-1.2.0/birdsong/blocks.py` & `wagtail_birdsong-2.0.0/birdsong/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-birdsong-1.2.0/birdsong/migrations/0001_initial.py` & `wagtail_birdsong-2.0.0/birdsong/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-birdsong-1.2.0/birdsong/migrations/0002_auto_20200603_0206.py` & `wagtail_birdsong-2.0.0/birdsong/migrations/0002_auto_20200603_0206.py`

 * *Files identical despite different names*

### Comparing `wagtail-birdsong-1.2.0/birdsong/migrations/0004_campaign_status.py` & `wagtail_birdsong-2.0.0/birdsong/migrations/0004_campaign_status.py`

 * *Files identical despite different names*

### Comparing `wagtail-birdsong-1.2.0/birdsong/migrations/0006_auto_20220428_0558.py` & `wagtail_birdsong-2.0.0/birdsong/migrations/0006_auto_20220428_0558.py`

 * *Files identical despite different names*

### Comparing `wagtail-birdsong-1.2.0/birdsong/migrations/0007_alter_contacttag_tag.py` & `wagtail_birdsong-2.0.0/birdsong/migrations/0007_alter_contacttag_tag.py`

 * *Files identical despite different names*

### Comparing `wagtail-birdsong-1.2.0/birdsong/migrations/0008_translation_support.py` & `wagtail_birdsong-2.0.0/birdsong/migrations/0008_translation_support.py`

 * *Files identical despite different names*

### Comparing `wagtail-birdsong-1.2.0/birdsong/models.py` & `wagtail_birdsong-2.0.0/birdsong/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,18 +72,22 @@
 
     def __str__(self):
         return self.name
 
     def get_template(self, request):
         return "mail/%s.html" % (camelcase_to_underscore(self.__class__.__name__))
 
+    def get_text_template(self, request):
+        return "mail/%s.txt" % (camelcase_to_underscore(self.__class__.__name__))
+
     def get_context(self, request, contact):
         site = Site.find_for_request(request)
         return {
             "self": self,
+            "request": request,
             "contact": contact,
             "site": site,
         }
 
 
 class Receipt(models.Model):
     campaign = models.ForeignKey(Campaign, on_delete=models.CASCADE)
```

### Comparing `wagtail-birdsong-1.2.0/birdsong/options.py` & `wagtail_birdsong-2.0.0/birdsong/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from django.conf import settings
 from django.forms import modelform_factory
 from django.http.response import HttpResponseRedirect
 from django.urls import re_path
 from django.utils.module_loading import import_string
 from django.utils.translation import gettext as _
 from django.utils.translation import pgettext
-from wagtail.contrib.modeladmin.helpers import AdminURLHelper, ButtonHelper
-from wagtail.contrib.modeladmin.options import ModelAdmin
+from wagtail_modeladmin.helpers import AdminURLHelper, ButtonHelper
+from wagtail_modeladmin.options import ModelAdmin
 
 from birdsong.conf import BIRDSONG_TEST_CONTACT
 
 from .models import CampaignStatus, Contact
 from .views import actions
 from .views import editor as editor_views
```

### Comparing `wagtail-birdsong-1.2.0/birdsong/static/birdsong/js/preview_campaign.js` & `wagtail_birdsong-2.0.0/birdsong/static/birdsong/js/preview_campaign.js`

 * *Files identical despite different names*

### Comparing `wagtail-birdsong-1.2.0/birdsong/templates/birdsong/editor/create_campaign.html` & `wagtail_birdsong-2.0.0/birdsong/templates/birdsong/editor/create_campaign.html`

 * *Files identical despite different names*

### Comparing `wagtail-birdsong-1.2.0/birdsong/templates/birdsong/editor/edit_campaign.html` & `wagtail_birdsong-2.0.0/birdsong/templates/birdsong/editor/edit_campaign.html`

 * *Files identical despite different names*

### Comparing `wagtail-birdsong-1.2.0/birdsong/templates/birdsong/editor/inspect_campaign.html` & `wagtail_birdsong-2.0.0/birdsong/templates/birdsong/editor/inspect_campaign.html`

 * *Files identical despite different names*

### Comparing `wagtail-birdsong-1.2.0/birdsong/templates/birdsong/editor/send_confirm.html` & `wagtail_birdsong-2.0.0/birdsong/templates/birdsong/editor/send_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail-birdsong-1.2.0/birdsong/templates/birdsong/editor/test_confirm.html` & `wagtail_birdsong-2.0.0/birdsong/templates/birdsong/editor/test_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail-birdsong-1.2.0/birdsong/utils.py` & `wagtail_birdsong-2.0.0/birdsong/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,13 +9,17 @@
     connection = connection or get_connection(
         username=auth_user,
         password=auth_password,
         fail_silently=fail_silently,
     )
 
     def _email_from_dict(data):
+        if 'html_body' not in data:
+            html_body = data.pop('body')
+        else:
+            html_body = data.pop('html_body')
         msg = EmailMultiAlternatives(connection=connection, **data)
-        msg.attach_alternative(data['body'], "text/html")
+        msg.attach_alternative(html_body, "text/html")
         return msg
 
     messages = [_email_from_dict(d) for d in email_data]
     return connection.send_messages(messages)
```

### Comparing `wagtail-birdsong-1.2.0/birdsong/views/actions.py` & `wagtail_birdsong-2.0.0/birdsong/views/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.contrib import messages
 from django.shortcuts import redirect
 from django.utils.translation import gettext as _
-from wagtail.contrib.modeladmin.helpers.url import AdminURLHelper
+from wagtail_modeladmin.helpers.url import AdminURLHelper
 
 from birdsong.models import CampaignStatus
 
 
 def redirect_helper(campaign):
     url_helper = AdminURLHelper(type(campaign))
     campaign_list_url = url_helper.get_action_url('index')
```

### Comparing `wagtail-birdsong-1.2.0/birdsong/views/editor.py` & `wagtail_birdsong-2.0.0/birdsong/views/editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.http.response import JsonResponse
 from django.shortcuts import render
 from django.template.loader import render_to_string
-from wagtail.contrib.modeladmin.views import CreateView, EditView, InspectView
+from wagtail_modeladmin.views import CreateView, EditView, InspectView
 
 from birdsong.conf import BIRDSONG_TEST_CONTACT
 
 
 def preview(request, campaign, test_contact):
     return render(
         request,
```

### Comparing `wagtail-birdsong-1.2.0/birdsong/views/unsubscribe.py` & `wagtail_birdsong-2.0.0/birdsong/views/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `wagtail-birdsong-1.2.0/birdsong/wagtail_hooks.py` & `wagtail_birdsong-2.0.0/birdsong/wagtail_hooks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from wagtail.contrib.modeladmin.options import (ModelAdmin, ModelAdminGroup,
-                                                hooks, modeladmin_register)
+from wagtail_modeladmin.options import (ModelAdmin, ModelAdminGroup, hooks,
+                                        modeladmin_register)
 
 from birdsong.conf import BIRDSONG_ADMIN_GROUP
 from birdsong.models import Campaign, Contact
 from birdsong.options import CampaignAdmin
 
 
 @hooks.register("register_icons")
@@ -69,18 +69,18 @@
     for example:
         from birdsong.wagtail_hooks import BirdsongAdminGroup, modeladmin_re_register
         @modeladmin_re_register
         class BirdsongAdminGroup(BirdsongAdminGroup):
             menu_icon = "mail"
 
     :param modeladmin_class: ModelAdmin class to re-register
-    :type modeladmin_class: class:`wagtail.contrib.modeladmin.options.ModelAdminGroup`
+    :type modeladmin_class: class:`wagtail_modeladmin.options.ModelAdminGroup`
 
     :return: Re-registered ModelAdmin class
-    :rtype: class:class:`wagtail.contrib.modeladmin.options.ModelAdminGroup`
+    :rtype: class:class:`wagtail_modeladmin.options.ModelAdminGroup`
     """
 
     @hooks.register("construct_main_menu")
     def unregister_menu_item(request, menu_items):
         if (
             modeladmin_class.menu_item_name
         ):  # menu_item_name defined or inherited by modeladmin_class?
```

### Comparing `wagtail-birdsong-1.2.0/setup.py` & `wagtail_birdsong-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     name="wagtail-birdsong",
     version=version,
     description="Create and send email campaigns from Wagtail",
     long_description=readme,
     author="Neon Jungle",
     author_email="developers@neonjungle.studio",
     install_requires=[
-        "wagtail>=4.1",
+        "wagtail>=5.2",
+        "wagtail-modeladmin",
         "django-mjml",
     ],
     setup_requires=["wheel"],
     zip_safe=False,
     license="BSD License",
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
```

### Comparing `wagtail-birdsong-1.2.0/tests/test_admin.py` & `wagtail_birdsong-2.0.0/tests/test_admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,30 +29,30 @@
         post_data.update(overrides)
         return nested_form_data(post_data)
 
     def test_create(self):
         response = self.client.post(
             "/admin/app/salecampaign/create/", self.post_data(), follow=True
         )
-        self.assertEquals(response.status_code, 200)
+        self.assertEqual(response.status_code, 200)
 
     def test_edit(self):
         response = self.client.post(
             f"/admin/app/salecampaign/edit/{self.campaign.id}/",
             self.post_data(overrides={"name": "A Different Name"}),
             follow=True,
         )
-        self.assertEquals(response.status_code, 200)
+        self.assertEqual(response.status_code, 200)
         self.assertContains(response, "A Different Name")
 
     def test_preview(self):
         response = self.client.get(
             f"/admin/app/salecampaign/preview/{self.campaign.id}/",
         )
-        self.assertEquals(response.status_code, 200)
+        self.assertEqual(response.status_code, 200)
         self.assertContains(response, "<p>The body</p>")
 
     def test_live_preview(self):
         # TODO (post with ajax headers?)
         pass
 
 
@@ -81,21 +81,22 @@
             {
                 "email": "have@email.com",
                 "first_name": "Find",
                 "last_name": "Me",
                 "location": "Moon",
             },
         )
-        sleep(10)  # Allow time  to send
+        sleep(3)  # Allow time  to send
         self.assertEqual(len(mail.outbox), 1)
-        self.assertTrue("Hi Find Me" in mail.outbox[0].body)
+        self.assertTrue("Hi Find Me" in str(mail.outbox[0].message()))
+        self.campaign.refresh_from_db()
         self.assertNotEqual(self.campaign.status, CampaignStatus.SENT)
 
     def test_send(self):
         self.client.get(f"/admin/app/salecampaign/send_campaign/{self.campaign.id}/")
 
-        sleep(10)  # Allow time  to send
-        self.assertEquals(len(mail.outbox), 2)
-        self.assertEquals(self.campaign.receipts.all().count(), 2)
+        sleep(3)  # Allow time  to send
+        self.assertEqual(len(mail.outbox), 2)
+        self.assertEqual(self.campaign.receipts.all().count(), 2)
         # Get fresh from db (altered in a thread)
-        fresh_campaign = SaleCampaign.objects.get(pk=self.campaign.pk)
-        self.assertEquals(fresh_campaign.status, CampaignStatus.SENT)
+        self.campaign.refresh_from_db()
+        self.assertEqual(self.campaign.status, CampaignStatus.SENT)
```

### Comparing `wagtail-birdsong-1.2.0/wagtail_birdsong.egg-info/PKG-INFO` & `wagtail_birdsong-2.0.0/wagtail_birdsong.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-birdsong
-Version: 1.2.0
+Version: 2.0.0
 Summary: Create and send email campaigns from Wagtail
 Author: Neon Jungle
 Author-email: developers@neonjungle.studio
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,16 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: BSD License
 License-File: LICENSE
-Requires-Dist: wagtail>=4.1
+Requires-Dist: wagtail>=5.2
+Requires-Dist: wagtail-modeladmin
 Requires-Dist: django-mjml
 
 .. image:: docs/birdsong.svg
     :width: 400
     :alt: Birdsong Logo
 
 A plugin for wagtail that allows you to create, send, preview, edit and test email campaigns from within Wagtail.
@@ -47,15 +48,15 @@
 
 .. code-block:: python
 
     INSTALLED_APPS = [
         ...
         'mjml',
         'birdsong',
-        'wagtail.contrib.modeladmin',
+        'wagtail_modeladmin',
         ...
     ]
 
 Make a new app e.g. ``email``, create a ``models.py`` with a model that extends the included ``Campaign`` model. Some compatible mjml streamfield blocks are included in birdsong for convenience.
 
 ``models.py``
```

### Comparing `wagtail-birdsong-1.2.0/wagtail_birdsong.egg-info/SOURCES.txt` & `wagtail_birdsong-2.0.0/wagtail_birdsong.egg-info/SOURCES.txt`

 * *Files identical despite different names*

