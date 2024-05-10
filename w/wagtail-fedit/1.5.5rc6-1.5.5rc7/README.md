# Comparing `tmp/wagtail_fedit-1.5.5rc6.tar.gz` & `tmp/wagtail_fedit-1.5.5rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.5rc6.tar", last modified: Fri May 10 12:10:23 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.5rc7.tar", last modified: Fri May 10 13:02:03 2024, max compression
```

## Comparing `wagtail_fedit-1.5.5rc6.tar` & `wagtail_fedit-1.5.5rc7.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.969414 wagtail_fedit-1.5.5rc6/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc6/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc6/MANIFEST.in
--rw-rw-rw-   0        0        0     3013 2024-05-10 12:10:23.970413 wagtail_fedit-1.5.5rc6/PKG-INFO
--rw-rw-rw-   0        0        0     1812 2024-04-28 14:18:11.000000 wagtail_fedit-1.5.5rc6/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc6/pyproject.toml
--rw-rw-rw-   0        0        0     1189 2024-05-10 12:10:23.971413 wagtail_fedit-1.5.5rc6/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.887660 wagtail_fedit-1.5.5rc6/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.901436 wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      532 2024-04-22 21:01:35.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0    14469 2024-04-25 18:57:33.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     6545 2024-04-25 18:29:05.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8652 2024-04-23 18:12:26.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     2305 2024-04-25 18:28:58.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2755 2024-04-25 18:28:49.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     5607 2024-05-07 18:13:59.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/models.py
--rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/apps.py
--rw-rw-rw-   0        0        0     1354 2024-04-25 09:55:56.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.903435 wagtail_fedit-1.5.5rc6/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.862026 wagtail_fedit-1.5.5rc6/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.862026 wagtail_fedit-1.5.5rc6/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.904430 wagtail_fedit-1.5.5rc6/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7262 2024-04-23 15:50:58.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    15296 2024-04-25 14:19:13.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.906129 wagtail_fedit-1.5.5rc6/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.906129 wagtail_fedit-1.5.5rc6/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0     1626 2024-04-25 13:40:59.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.862026 wagtail_fedit-1.5.5rc6/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.862026 wagtail_fedit-1.5.5rc6/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.908130 wagtail_fedit-1.5.5rc6/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5745 2024-05-08 11:26:45.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.910128 wagtail_fedit-1.5.5rc6/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    51061 2024-05-08 13:42:06.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/static/wagtail_fedit/js/edit.js
--rw-rw-rw-   0        0        0    26914 2024-05-07 17:43:52.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.910753 wagtail_fedit-1.5.5rc6/wagtail_fedit/static/wagtail_fedit/js/licenses/
--rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.867142 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.912096 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.912096 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.916466 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      571 2024-05-08 11:29:32.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.921971 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
--rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
--rw-rw-rw-   0        0        0      555 2024-04-21 21:13:45.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
--rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
--rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.926294 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.928596 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.928596 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.933742 wagtail_fedit-1.5.5rc6/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.935453 wagtail_fedit-1.5.5rc6/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    13140 2024-05-08 09:22:37.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    10310 2024-05-07 21:59:17.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.936460 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.938512 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.942341 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.951853 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     8962 2024-04-25 13:24:28.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    28117 2024-04-25 18:07:06.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/test_model_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.956076 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0     1196 2024-04-23 17:25:08.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    18101 2024-04-25 13:15:30.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.960078 wagtail_fedit-1.5.5rc6/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8490 2024-04-25 13:06:47.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17778 2024-04-25 09:19:32.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     2239 2024-04-25 09:52:47.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.969414 wagtail_fedit-1.5.5rc6/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1766 2024-05-10 12:07:48.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     2446 2024-05-07 21:59:49.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      328 2024-04-21 16:44:33.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     3100 2024-05-07 18:11:10.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7637 2024-04-23 20:17:24.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:10:23.891854 wagtail_fedit-1.5.5rc6/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     3013 2024-05-10 12:10:23.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4466 2024-05-10 12:10:23.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 12:10:23.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-10 12:10:23.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-10 12:10:23.000000 wagtail_fedit-1.5.5rc6/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.461602 wagtail_fedit-1.5.5rc7/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3013 2024-05-10 13:02:03.462604 wagtail_fedit-1.5.5rc7/PKG-INFO
+-rw-rw-rw-   0        0        0     1812 2024-04-28 14:18:11.000000 wagtail_fedit-1.5.5rc7/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-05-10 13:02:03.463603 wagtail_fedit-1.5.5rc7/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.341659 wagtail_fedit-1.5.5rc7/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.362425 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      532 2024-04-22 21:01:35.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    14469 2024-04-25 18:57:33.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     6545 2024-04-25 18:29:05.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8652 2024-04-23 18:12:26.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     2305 2024-04-25 18:28:58.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2755 2024-04-25 18:28:49.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     5607 2024-05-07 18:13:59.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/models.py
+-rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/apps.py
+-rw-rw-rw-   0        0        0     1354 2024-04-25 09:55:56.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.368428 wagtail_fedit-1.5.5rc7/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.316636 wagtail_fedit-1.5.5rc7/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.316636 wagtail_fedit-1.5.5rc7/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.371240 wagtail_fedit-1.5.5rc7/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7262 2024-04-23 15:50:58.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    15296 2024-04-25 14:19:13.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.371240 wagtail_fedit-1.5.5rc7/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.372248 wagtail_fedit-1.5.5rc7/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0     1626 2024-04-25 13:40:59.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.319127 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.320129 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.375889 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5745 2024-05-08 11:26:45.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.377068 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    51061 2024-05-08 13:42:06.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/js/edit.js
+-rw-rw-rw-   0        0        0    26914 2024-05-07 17:43:52.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.378075 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/js/licenses/
+-rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.321128 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.380070 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.381069 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.384942 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      571 2024-05-08 11:29:32.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.397329 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
+-rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
+-rw-rw-rw-   0        0        0      555 2024-04-21 21:13:45.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.404320 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.407347 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.408540 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.410532 wagtail_fedit-1.5.5rc7/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.412534 wagtail_fedit-1.5.5rc7/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13140 2024-05-08 09:22:37.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10310 2024-05-07 21:59:17.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.415532 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.421320 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.424174 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.439129 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     8962 2024-04-25 13:24:28.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    28117 2024-04-25 18:07:06.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_model_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.444444 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0     1196 2024-04-23 17:25:08.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    18101 2024-04-25 13:15:30.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.450602 wagtail_fedit-1.5.5rc7/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8490 2024-04-25 13:06:47.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17778 2024-04-25 09:19:32.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     2239 2024-04-25 09:52:47.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.460610 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1832 2024-05-10 12:39:02.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     2446 2024-05-07 21:59:49.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      328 2024-04-21 16:44:33.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     3100 2024-05-07 18:11:10.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7637 2024-04-23 20:17:24.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.348335 wagtail_fedit-1.5.5rc7/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     3013 2024-05-10 13:02:03.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4466 2024-05-10 13:02:03.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 13:02:03.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-10 13:02:03.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-10 13:02:03.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.5rc6/LICENSE` & `wagtail_fedit-1.5.5rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/PKG-INFO` & `wagtail_fedit-1.5.5rc7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.5rc6
+Version: 1.5.5rc7
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_fedit-1.5.5rc6/README.md` & `wagtail_fedit-1.5.5rc7/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/setup.cfg` & `wagtail_fedit-1.5.5rc7/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3572 6336 0d0a 6465 7363 7269 7074 696f  5rc6..descriptio
+00000030: 3572 6337 0d0a 6465 7363 7269 7074 696f  5rc7..descriptio
 00000040: 6e20 3d20 4672 6f6e 7465 6e64 2065 6469  n = Frontend edi
 00000050: 7469 6e67 2066 6f72 2079 6f75 7220 5761  ting for your Wa
 00000060: 6774 6169 6c20 7369 7465 0d0a 6c6f 6e67  gtail site..long
 00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type =
```

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/__init__.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/block.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/funcs.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/misc.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/models.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/errors.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/errors.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/models.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/settings.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/static/wagtail_fedit/js/edit.js` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/js/edit.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/test_model_edit.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_model_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/views/adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 
 class WagtailFEditActionMenuItemMixin:
     name = 'action-frontend-edit'
     label = _('Frontend Edit')
     icon_name = "desktop"
 
     def is_shown(self, context):
-        instance = context.get("instance", context["page"])
+        instance = context.get("instance", context.get("page", None))
+        if instance is None:
+            return False
 
         for hook in hooks.get_hooks(ACTION_MENU_ITEM_IS_SHOWN):
             result = hook(context, instance)
             if result is not None:
                 return result
 
         return context["view"] == "edit"\
```

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.5rc7/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.5.5rc6
+Version: 1.5.5rc7
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_fedit-1.5.5rc6/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.5rc7/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

