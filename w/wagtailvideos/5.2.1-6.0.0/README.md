# Comparing `tmp/wagtailvideos-5.2.1.tar.gz` & `tmp/wagtailvideos-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailvideos-5.2.1.tar", last modified: Mon Jan  8 22:53:11 2024, max compression
+gzip compressed data, was "wagtailvideos-6.0.0.tar", last modified: Fri May 10 05:29:03 2024, max compression
```

## Comparing `wagtailvideos-5.2.1.tar` & `wagtailvideos-6.0.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.767634 wagtailvideos-5.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1481 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6092 2024-01-08 22:53:11.767634 wagtailvideos-5.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5031 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      295 2024-01-08 22:53:11.768634 wagtailvideos-5.2.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1386 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.752635 wagtailvideos-5.2.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.753635 wagtailvideos-5.2.1/tests/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/tests/app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.754635 wagtailvideos-5.2.1/tests/app/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    32030 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/tests/app/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/tests/app/migrations/0002_alter_testpage_video_streamfield.py
--rw-rw-rw-   0 root         (0) root         (0)    27639 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/tests/app/migrations/0003_alter_customvideotrack_file_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/tests/app/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/tests/app/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2218 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/tests/app/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/tests/app/test_block.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/tests/app/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     6455 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/tests/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    25977 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/tests/test_admin_views.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/tests/test_custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1628 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/tests/test_template_tag.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.757634 wagtailvideos-5.2.1/wagtailvideos/
--rw-rw-rw-   0 root         (0) root         (0)      846 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/blocks.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/edit_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     2136 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/ffmpeg.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     3206 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      637 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/jinja2tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.747635 wagtailvideos-5.2.1/wagtailvideos/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.748635 wagtailvideos-5.2.1/wagtailvideos/locale/ru_RU/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.758635 wagtailvideos-5.2.1/wagtailvideos/locale/ru_RU/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     9219 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    13787 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.762635 wagtailvideos-5.2.1/wagtailvideos/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1966 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      757 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/migrations/0002_auto_20160321_1610.py
--rw-rw-rw-   0 root         (0) root         (0)     1273 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/migrations/0003_auto_20160705_1646.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/migrations/0004_auto_20160706_1153.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/migrations/0005_videotranscode_error_message.py
--rw-rw-rw-   0 root         (0) root         (0)      585 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/migrations/0006_auto_20160707_1413.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/migrations/0007_video_duration.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/migrations/0008_auto_20160728_1523.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/migrations/0009_videotranscode_quality.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/migrations/0010_video_ordering.py
--rw-rw-rw-   0 root         (0) root         (0)    28229 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/migrations/0011_video_tracks.py
--rw-rw-rw-   0 root         (0) root         (0)    26753 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/migrations/0012_remove_unique_constraint.py
--rw-rw-rw-   0 root         (0) root         (0)     3473 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/migrations/0013_add_choose_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)    44986 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13904 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/models.py
--rw-rw-rw-   0 root         (0) root         (0)      322 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     2642 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.748635 wagtailvideos-5.2.1/wagtailvideos/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.749635 wagtailvideos-5.2.1/wagtailvideos/static/wagtailvideos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.762635 wagtailvideos-5.2.1/wagtailvideos/static/wagtailvideos/css/
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/static/wagtailvideos/css/edit-video.css
--rw-rw-rw-   0 root         (0) root         (0)      364 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/static/wagtailvideos/css/summary-override.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.762635 wagtailvideos-5.2.1/wagtailvideos/static/wagtailvideos/js/
--rw-rw-rw-   0 root         (0) root         (0)     5536 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/static/wagtailvideos/js/add-multiple.js
--rw-rw-rw-   0 root         (0) root         (0)      316 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/static/wagtailvideos/js/video-chooser-telepath.js
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/static/wagtailvideos/js/video-chooser.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.749635 wagtailvideos-5.2.1/wagtailvideos/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.750635 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.763635 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/chooser/
--rw-rw-rw-   0 root         (0) root         (0)      926 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/chooser/chooser.html
--rw-rw-rw-   0 root         (0) root         (0)     1988 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/chooser/results.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.763635 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/homepage/
--rw-rw-rw-   0 root         (0) root         (0)      480 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/homepage/videos_summary.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.763635 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/multiple/
--rw-rw-rw-   0 root         (0) root         (0)     4414 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/multiple/add.html
--rw-rw-rw-   0 root         (0) root         (0)     1042 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.749635 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/permissions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.764634 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/permissions/includes/
--rw-rw-rw-   0 root         (0) root         (0)      253 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/permissions/includes/video_permissions_formset.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.765634 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/videos/
--rw-rw-rw-   0 root         (0) root         (0)      246 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/videos/_file_field.html
--rw-rw-rw-   0 root         (0) root         (0)      232 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/videos/_file_field_as_li.html
--rw-rw-rw-   0 root         (0) root         (0)     1222 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/videos/add.html
--rw-rw-rw-   0 root         (0) root         (0)      820 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html
--rw-rw-rw-   0 root         (0) root         (0)     6806 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/videos/edit.html
--rw-rw-rw-   0 root         (0) root         (0)     1393 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/videos/index.html
--rw-rw-rw-   0 root         (0) root         (0)     2019 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/videos/results.html
--rw-rw-rw-   0 root         (0) root         (0)     1903 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/videos/usage.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.765634 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/widgets/
--rw-rw-rw-   0 root         (0) root         (0)      442 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/widgets/video_chooser.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.766635 wagtailvideos-5.2.1/wagtailvideos/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/templatetags/wagtailvideos_tags.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.767634 wagtailvideos-5.2.1/wagtailvideos/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5285 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/views/chooser.py
--rw-rw-rw-   0 root         (0) root         (0)     4730 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/views/multiple.py
--rw-rw-rw-   0 root         (0) root         (0)     7693 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/views/videos.py
--rw-rw-rw-   0 root         (0) root         (0)     4303 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/wagtail_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     2085 2024-01-08 22:53:03.000000 wagtailvideos-5.2.1/wagtailvideos/widgets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-08 22:53:11.767634 wagtailvideos-5.2.1/wagtailvideos.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6092 2024-01-08 22:53:11.000000 wagtailvideos-5.2.1/wagtailvideos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3389 2024-01-08 22:53:11.000000 wagtailvideos-5.2.1/wagtailvideos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-08 22:53:11.000000 wagtailvideos-5.2.1/wagtailvideos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-08 22:53:11.000000 wagtailvideos-5.2.1/wagtailvideos.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       91 2024-01-08 22:53:11.000000 wagtailvideos-5.2.1/wagtailvideos.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-01-08 22:53:11.000000 wagtailvideos-5.2.1/wagtailvideos.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.571055 wagtailvideos-6.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1481 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6054 2024-05-10 05:29:03.571055 wagtailvideos-6.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      295 2024-05-10 05:29:03.571055 wagtailvideos-6.0.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1373 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.556055 wagtailvideos-6.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.557055 wagtailvideos-6.0.0/tests/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.558055 wagtailvideos-6.0.0/tests/app/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    32030 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/migrations/0002_alter_testpage_video_streamfield.py
+-rw-rw-rw-   0 root         (0) root         (0)    27639 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/migrations/0003_alter_customvideotrack_file_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2210 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/test_block.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/app/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     6455 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    25986 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/test_admin_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/test_custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1628 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/test_template_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.560055 wagtailvideos-6.0.0/wagtailvideos/
+-rw-rw-rw-   0 root         (0) root         (0)      838 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/edit_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2136 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/ffmpeg.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     3206 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      637 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/jinja2tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.551055 wagtailvideos-6.0.0/wagtailvideos/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.552055 wagtailvideos-6.0.0/wagtailvideos/locale/ru_RU/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.562055 wagtailvideos-6.0.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     9219 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    13787 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.565055 wagtailvideos-6.0.0/wagtailvideos/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      757 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0002_auto_20160321_1610.py
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0003_auto_20160705_1646.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0004_auto_20160706_1153.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0005_videotranscode_error_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      585 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0006_auto_20160707_1413.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0007_video_duration.py
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0008_auto_20160728_1523.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0009_videotranscode_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0010_video_ordering.py
+-rw-rw-rw-   0 root         (0) root         (0)    28229 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0011_video_tracks.py
+-rw-rw-rw-   0 root         (0) root         (0)    26753 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0012_remove_unique_constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3473 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0013_add_choose_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)    44986 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13904 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2642 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.552055 wagtailvideos-6.0.0/wagtailvideos/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.552055 wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.565055 wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/css/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/css/edit-video.css
+-rw-rw-rw-   0 root         (0) root         (0)      364 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/css/summary-override.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.566055 wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/js/
+-rw-rw-rw-   0 root         (0) root         (0)     5536 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/js/add-multiple.js
+-rw-rw-rw-   0 root         (0) root         (0)      316 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/js/video-chooser-telepath.js
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/js/video-chooser.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.552055 wagtailvideos-6.0.0/wagtailvideos/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.553055 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.566055 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/chooser/
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/chooser/chooser.html
+-rw-rw-rw-   0 root         (0) root         (0)     1988 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/chooser/results.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.567055 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/homepage/
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/homepage/videos_summary.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.567055 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/multiple/
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/multiple/add.html
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.553055 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/permissions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.567055 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/permissions/includes/
+-rw-rw-rw-   0 root         (0) root         (0)      253 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/permissions/includes/video_permissions_formset.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.569055 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/_file_field.html
+-rw-rw-rw-   0 root         (0) root         (0)      232 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/_file_field_as_li.html
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/add.html
+-rw-rw-rw-   0 root         (0) root         (0)      820 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html
+-rw-rw-rw-   0 root         (0) root         (0)     6815 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/edit.html
+-rw-rw-rw-   0 root         (0) root         (0)     1393 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     2019 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/results.html
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/usage.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.569055 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)      442 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/widgets/video_chooser.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.569055 wagtailvideos-6.0.0/wagtailvideos/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/templatetags/wagtailvideos_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.570055 wagtailvideos-6.0.0/wagtailvideos/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5285 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/views/chooser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4730 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/views/multiple.py
+-rw-rw-rw-   0 root         (0) root         (0)     7685 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/views/videos.py
+-rw-rw-rw-   0 root         (0) root         (0)     4295 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/wagtail_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2024-05-10 05:28:54.000000 wagtailvideos-6.0.0/wagtailvideos/widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 05:29:03.570055 wagtailvideos-6.0.0/wagtailvideos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6054 2024-05-10 05:29:03.000000 wagtailvideos-6.0.0/wagtailvideos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3389 2024-05-10 05:29:03.000000 wagtailvideos-6.0.0/wagtailvideos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 05:29:03.000000 wagtailvideos-6.0.0/wagtailvideos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 05:29:03.000000 wagtailvideos-6.0.0/wagtailvideos.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       94 2024-05-10 05:29:03.000000 wagtailvideos-6.0.0/wagtailvideos.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-10 05:29:03.000000 wagtailvideos-6.0.0/wagtailvideos.egg-info/top_level.txt
```

### Comparing `wagtailvideos-5.2.1/LICENSE` & `wagtailvideos-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/PKG-INFO` & `wagtailvideos-6.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailvideos
-Version: 5.2.1
+Version: 6.0.0
 Summary: A wagtail module for uploading and displaying videos in various codecs.
 Home-page: https://github.com/neon-jungle/wagtailvideos
 Author: Neon Jungle
 Author-email: developers@neonjungle.studio
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -19,16 +19,15 @@
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: BSD License
 License-File: LICENSE
 Requires-Dist: wagtail>=5.2
 Requires-Dist: Django>=3.2
 Requires-Dist: django-enumchoicefield>=1.1.0
 Requires-Dist: bcp47==0.0.4
-Provides-Extra: testing
-Requires-Dist: mock==2.0.0; extra == "testing"
+Requires-Dist: wagtail-modeladmin>=2.0.0
 
 wagtailvideos
 =============
 
 .. image:: https://gitlab.com/neonjungle/wagtailvideos/badges/master/pipeline.svg
     :target: https://gitlab.com/neonjungle/wagtailvideos/pipelines?ref=master
 
@@ -202,15 +201,15 @@
     class CustomVideoTrack(AbstractVideoTrack):
         listing = ParentalKey(CustomTrackListing, related_name='tracks', on_delete=models.CASCADE)
 
 
 Video text tracks:
 ~~~~~~~~~~~~~~~~~~
 
-To enable the uploading and displaying of VTT tracks (e.g. subtitles, captions) you'll need to add ``wagtail.contrib.modeladmin`` to your installed apps.
+To enable the uploading and displaying of VTT tracks (e.g. subtitles, captions) you'll need to add ``wagtail_modeladmin`` to your installed apps.
 Once added, there will be an new area in the admin for attaching VTT files to videos with associaled metadata.
 
 Future features
 ---------------
 
 -  Some docs
 -  Richtext embed
```

### Comparing `wagtailvideos-5.2.1/README.rst` & `wagtailvideos-6.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
     class CustomVideoTrack(AbstractVideoTrack):
         listing = ParentalKey(CustomTrackListing, related_name='tracks', on_delete=models.CASCADE)
 
 
 Video text tracks:
 ~~~~~~~~~~~~~~~~~~
 
-To enable the uploading and displaying of VTT tracks (e.g. subtitles, captions) you'll need to add ``wagtail.contrib.modeladmin`` to your installed apps.
+To enable the uploading and displaying of VTT tracks (e.g. subtitles, captions) you'll need to add ``wagtail_modeladmin`` to your installed apps.
 Once added, there will be an new area in the admin for attaching VTT files to videos with associaled metadata.
 
 Future features
 ---------------
 
 -  Some docs
 -  Richtext embed
```

### Comparing `wagtailvideos-5.2.1/setup.py` & `wagtailvideos-6.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 with open("README.rst", "r") as f:
     readme = f.read()
 
 from setuptools import find_packages, setup  # noqa: E4
 
 setup(
     name="wagtailvideos",
-    version="5.2.1",
+    version="6.0.0",
     description="A wagtail module for uploading and displaying videos in various codecs.",
     long_description=readme,
     author="Neon Jungle",
     author_email="developers@neonjungle.studio",
     url="https://github.com/neon-jungle/wagtailvideos",
     install_requires=[
         "wagtail>=5.2",
         "Django>=3.2",
         "django-enumchoicefield>=1.1.0",
         "bcp47==0.0.4",
+        "wagtail-modeladmin>=2.0.0"
     ],
-    extras_require={"testing": ["mock==2.0.0"]},
     zip_safe=False,
     license="BSD License",
     packages=find_packages(),
     include_package_data=True,
     package_data={},
     classifiers=[
         "Environment :: Web Environment",
```

### Comparing `wagtailvideos-5.2.1/tests/app/migrations/0001_initial.py` & `wagtailvideos-6.0.0/tests/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/tests/app/migrations/0003_alter_customvideotrack_file_and_more.py` & `wagtailvideos-6.0.0/tests/app/migrations/0003_alter_customvideotrack_file_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/tests/app/models.py` & `wagtailvideos-6.0.0/tests/app/models.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/tests/app/settings.py` & `wagtailvideos-6.0.0/tests/app/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "wagtail",
     "wagtail.admin",
     "wagtail.users",
     "wagtail.sites",
     "wagtail.snippets",
     "wagtail.images",
     "wagtail.documents",
-    "wagtail.contrib.modeladmin",
+    "wagtail_modeladmin",
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.messages",
     "django.contrib.sessions",
     "django.contrib.staticfiles",
 ]
```

### Comparing `wagtailvideos-5.2.1/tests/app/test_block.py` & `wagtailvideos-6.0.0/tests/app/test_block.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/tests/app/urls.py` & `wagtailvideos-6.0.0/tests/app/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/tests/storage.py` & `wagtailvideos-6.0.0/tests/storage.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/tests/test_admin_views.py` & `wagtailvideos-6.0.0/tests/test_admin_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
+from unittest.mock import patch
 
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Group, Permission
 from django.core.files.uploadedfile import SimpleUploadedFile
 from django.template.defaultfilters import filesizeformat
 from django.test import TestCase, override_settings
 from django.urls import reverse
-from mock import patch
 from wagtail.models import Collection, GroupCollectionPermission
 from wagtail.test.utils import WagtailTestUtils
 
 from tests.utils import create_test_video_file
 from wagtailvideos.models import Video
```

### Comparing `wagtailvideos-5.2.1/tests/test_custom_model.py` & `wagtailvideos-6.0.0/tests/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/tests/test_template_tag.py` & `wagtailvideos-6.0.0/tests/test_template_tag.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/__init__.py` & `wagtailvideos-6.0.0/wagtailvideos/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from django.core.exceptions import ImproperlyConfigured
 
 default_app_config = 'wagtailvideos.apps.WagtailVideosApp'
 
 
 def is_modeladmin_installed():
     from django.apps import apps
-    return apps.is_installed('wagtail.contrib.modeladmin')
+    return apps.is_installed('wagtail_modeladmin')
 
 
 def get_video_model_string():
     return getattr(settings, 'WAGTAILVIDEOS_VIDEO_MODEL', 'wagtailvideos.Video')
 
 
 def get_video_model():
```

### Comparing `wagtailvideos-5.2.1/wagtailvideos/apps.py` & `wagtailvideos-6.0.0/wagtailvideos/apps.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/blocks.py` & `wagtailvideos-6.0.0/wagtailvideos/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/ffmpeg.py` & `wagtailvideos-6.0.0/wagtailvideos/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/fields.py` & `wagtailvideos-6.0.0/wagtailvideos/fields.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/forms.py` & `wagtailvideos-6.0.0/wagtailvideos/forms.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/jinja2tags.py` & `wagtailvideos-6.0.0/wagtailvideos/jinja2tags.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.mo` & `wagtailvideos-6.0.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.po` & `wagtailvideos-6.0.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/migrations/0001_initial.py` & `wagtailvideos-6.0.0/wagtailvideos/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/migrations/0002_auto_20160321_1610.py` & `wagtailvideos-6.0.0/wagtailvideos/migrations/0002_auto_20160321_1610.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/migrations/0003_auto_20160705_1646.py` & `wagtailvideos-6.0.0/wagtailvideos/migrations/0003_auto_20160705_1646.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/migrations/0004_auto_20160706_1153.py` & `wagtailvideos-6.0.0/wagtailvideos/migrations/0004_auto_20160706_1153.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/migrations/0006_auto_20160707_1413.py` & `wagtailvideos-6.0.0/wagtailvideos/migrations/0006_auto_20160707_1413.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/migrations/0009_videotranscode_quality.py` & `wagtailvideos-6.0.0/wagtailvideos/migrations/0009_videotranscode_quality.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/migrations/0011_video_tracks.py` & `wagtailvideos-6.0.0/wagtailvideos/migrations/0011_video_tracks.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/migrations/0012_remove_unique_constraint.py` & `wagtailvideos-6.0.0/wagtailvideos/migrations/0012_remove_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/migrations/0013_add_choose_permissions.py` & `wagtailvideos-6.0.0/wagtailvideos/migrations/0013_add_choose_permissions.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py` & `wagtailvideos-6.0.0/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/models.py` & `wagtailvideos-6.0.0/wagtailvideos/models.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/signals.py` & `wagtailvideos-6.0.0/wagtailvideos/signals.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/static/wagtailvideos/js/add-multiple.js` & `wagtailvideos-6.0.0/wagtailvideos/static/wagtailvideos/js/add-multiple.js`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/chooser/chooser.html` & `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/chooser/chooser.html`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         action="{{ results_url }}"
         method="GET"
         autocomplete="off"
         novalidate
     >
         <ul class="fields">
             {% for field in filter_form %}
-                {% include "wagtailadmin/shared/field_as_li.html" with field=field %}
+                <li>{% include "wagtailadmin/shared/field.html" with field=field %}</li>
             {% endfor %}
             {% if popular_tags %}
                 <li class="taglist w-label-3">
                     <h3>{% trans 'Popular tags' %}</h3>
                     {% for tag in popular_tags %}
                         <a class="suggested-tag tag" href="{% url 'wagtailvideos:index' %}?tag={{ tag.name|urlencode }}">{{ tag.name }}</a>
                     {% endfor %}
```

### Comparing `wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/chooser/results.html` & `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/chooser/results.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/multiple/add.html` & `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/multiple/add.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html` & `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <form action="{% url 'wagtailvideos:edit_multiple' video.id %}" method="POST" enctype="multipart/form-data">
     <ul class="fields">
         {% csrf_token %}
         {% for field in form %}
             {% if field.is_hidden %}
                 {{ field }}
             {% else %}
-                {% include "wagtailadmin/shared/field_as_li.html" %}
+                <li>{% include "wagtailadmin/shared/field.html" %}</li>
             {% endif %}
         {% endfor %}
         <li>
             <input class="button" type="submit" value="{% trans 'Update' %}" />
             <a href="{% url 'wagtailvideos:delete_multiple' video.id %}" class="delete button button-secondary no">{% trans "Delete" %}</a>
         </li>
     </ul>
```

#### html2text {}

```diff
@@ -1,6 +1,7 @@
 {% load i18n %}
     * {% csrf_token %} {% for field in form %} {% if field.is_hidden %} {
-      { field }} {% else %} {% include "wagtailadmin/shared/field_as_li.html"
-      %} {% endif %} {% endfor %}
+      { field }} {% else %}
+    * {% include "wagtailadmin/shared/field.html" %}
+    * {% endif %} {% endfor %}
     * [{% trans 'Update' %}]_{_%_ _t_r_a_n_s_ _"_D_e_l_e_t_e_"_ _%_}
 {% if video.thumbnail %} [{% trans 'Video thumbnail' %}]{% endif %}
```

### Comparing `wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/videos/add.html` & `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/add.html`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         <form action="{% url 'wagtailvideos:add' %}" method="POST" enctype="multipart/form-data">
             {% csrf_token %}
             <ul class="fields">
                 {% for field in form %}
                     {% if field.is_hidden %}
                         {{ field }}
                     {% else %}
-                        {% include "wagtailadmin/shared/field_as_li.html" with field=field %}
+                        <li>{% include "wagtailadmin/shared/field.html" with field=field %}</li>
                     {% endif %}
                 {% endfor %}
                 <li><input class="button" type="submit" value="{% trans 'Save' %}" /></li>
             </ul>
         </form>
     </div>
 {% endblock %}
```

### Comparing `wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html` & `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/videos/edit.html` & `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/edit.html`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             <ul class="fields">
                 {% for field in form %}
                   {% if field.name == 'file' %}
                     {% include "wagtailvideos/videos/_file_field_as_li.html"  with li_classes="label-above label-uppercase" %}
                   {% elif field.is_hidden %}
                     {{ field }}
                   {% else %}
-                    {% include "wagtailadmin/shared/field_as_li.html" with li_classes="label-above label-uppercase" %}
+                    <li>{% include "wagtailadmin/shared/field.html" with li_classes="label-above label-uppercase" %}</li>
                   {% endif %}
                 {% endfor %}
                 <li>
                     <input type="submit" class="button" value="{% trans 'Save' %}" />
                     {% if user_can_delete %}
                         <a href="{% url 'wagtailvideos:delete' video.id %}" class="button button-secondary no">{% trans "Delete video" %}</a>
                     {% endif %}
@@ -105,16 +105,16 @@
                 {% endfor %}
             </ul>
             {% endif %}
             <h3 class="u-text-transform-uppercase">{% trans "Create transcode" %}</h3>
             <form action="{% url 'wagtailvideos:create_transcode' video.id %}" method="POST">
                 <ul class="fields">
                     {% csrf_token %}
-                    {% include "wagtailadmin/shared/field_as_li.html" with field=transcode_form.media_format li_classes="label-above label-uppercase" %}
-                    {% include "wagtailadmin/shared/field_as_li.html" with field=transcode_form.quality li_classes="label-above label-uppercase" %}
+                    <li>{% include "wagtailadmin/shared/field.html" with field=transcode_form.media_format li_classes="label-above label-uppercase" %}</li>
+                    <li>{% include "wagtailadmin/shared/field.html" with field=transcode_form.quality li_classes="label-above label-uppercase" %}</li>
                     <li>
                         <input class="button" type="submit" value="{% trans 'Start' %}" />
                     </li>
                 </ul>
             </form>
         {% else %}
             <br/><br/>
```

### Comparing `wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/videos/index.html` & `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/index.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/videos/results.html` & `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/results.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/templates/wagtailvideos/videos/usage.html` & `wagtailvideos-6.0.0/wagtailvideos/templates/wagtailvideos/videos/usage.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/templatetags/wagtailvideos_tags.py` & `wagtailvideos-6.0.0/wagtailvideos/templatetags/wagtailvideos_tags.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/urls.py` & `wagtailvideos-6.0.0/wagtailvideos/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/views/chooser.py` & `wagtailvideos-6.0.0/wagtailvideos/views/chooser.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/views/multiple.py` & `wagtailvideos-6.0.0/wagtailvideos/views/multiple.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos/views/videos.py` & `wagtailvideos-6.0.0/wagtailvideos/views/videos.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from django.utils.translation import gettext as _
 from django.views.decorators.http import require_POST
 from django.views.decorators.vary import vary_on_headers
 from wagtail.admin import messages
 from wagtail.admin.auth import PermissionPolicyChecker
 from wagtail.admin.forms.search import SearchForm
 from wagtail.admin.models import popular_tags_for_model
-from wagtail.contrib.modeladmin.helpers import AdminURLHelper
 from wagtail.models import Collection
 from wagtail.search.backends import get_search_backends
+from wagtail_modeladmin.helpers import AdminURLHelper
 
 from wagtailvideos import ffmpeg, get_video_model, is_modeladmin_installed
 from wagtailvideos.forms import VideoTranscodeAdminForm, get_video_form
 from wagtailvideos.permissions import permission_policy
 
 permission_checker = PermissionPolicyChecker(permission_policy)
```

### Comparing `wagtailvideos-5.2.1/wagtailvideos/wagtail_hooks.py` & `wagtailvideos-6.0.0/wagtailvideos/wagtail_hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from django.utils.html import format_html
 from django.utils.translation import gettext_lazy as _
 from wagtail import hooks
 from wagtail.admin.menu import Menu, MenuItem, SubmenuMenuItem
 from wagtail.admin.panels import InlinePanel
 from wagtail.admin.search import SearchArea
 from wagtail.admin.site_summary import SummaryItem
-from wagtail.contrib.modeladmin.options import ModelAdmin, modeladmin_register
+from wagtail_modeladmin.options import ModelAdmin, modeladmin_register
 
 from wagtailvideos import get_video_model, is_modeladmin_installed, urls
 from wagtailvideos.edit_handlers import VideoChooserPanel
 from wagtailvideos.forms import GroupVideoPermissionFormSet
 from wagtailvideos.views.chooser import viewset as chooser_viewset
 
 from .permissions import permission_policy
```

### Comparing `wagtailvideos-5.2.1/wagtailvideos/widgets.py` & `wagtailvideos-6.0.0/wagtailvideos/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-5.2.1/wagtailvideos.egg-info/PKG-INFO` & `wagtailvideos-6.0.0/wagtailvideos.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailvideos
-Version: 5.2.1
+Version: 6.0.0
 Summary: A wagtail module for uploading and displaying videos in various codecs.
 Home-page: https://github.com/neon-jungle/wagtailvideos
 Author: Neon Jungle
 Author-email: developers@neonjungle.studio
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -19,16 +19,15 @@
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: BSD License
 License-File: LICENSE
 Requires-Dist: wagtail>=5.2
 Requires-Dist: Django>=3.2
 Requires-Dist: django-enumchoicefield>=1.1.0
 Requires-Dist: bcp47==0.0.4
-Provides-Extra: testing
-Requires-Dist: mock==2.0.0; extra == "testing"
+Requires-Dist: wagtail-modeladmin>=2.0.0
 
 wagtailvideos
 =============
 
 .. image:: https://gitlab.com/neonjungle/wagtailvideos/badges/master/pipeline.svg
     :target: https://gitlab.com/neonjungle/wagtailvideos/pipelines?ref=master
 
@@ -202,15 +201,15 @@
     class CustomVideoTrack(AbstractVideoTrack):
         listing = ParentalKey(CustomTrackListing, related_name='tracks', on_delete=models.CASCADE)
 
 
 Video text tracks:
 ~~~~~~~~~~~~~~~~~~
 
-To enable the uploading and displaying of VTT tracks (e.g. subtitles, captions) you'll need to add ``wagtail.contrib.modeladmin`` to your installed apps.
+To enable the uploading and displaying of VTT tracks (e.g. subtitles, captions) you'll need to add ``wagtail_modeladmin`` to your installed apps.
 Once added, there will be an new area in the admin for attaching VTT files to videos with associaled metadata.
 
 Future features
 ---------------
 
 -  Some docs
 -  Richtext embed
```

### Comparing `wagtailvideos-5.2.1/wagtailvideos.egg-info/SOURCES.txt` & `wagtailvideos-6.0.0/wagtailvideos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

