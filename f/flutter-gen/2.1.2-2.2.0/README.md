# Comparing `tmp/flutter_gen-2.1.2.tar.gz` & `tmp/flutter_gen-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flutter_gen-2.1.2.tar", last modified: Fri Feb  2 09:44:40 2024, max compression
+gzip compressed data, was "flutter_gen-2.2.0.tar", last modified: Fri May 10 03:38:14 2024, max compression
```

## Comparing `flutter_gen-2.1.2.tar` & `flutter_gen-2.2.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.834103 flutter_gen-2.1.2/
--rw-r--r--   0 tienpx     (501) staff       (20)     1092 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/LICENSE
--rw-r--r--   0 tienpx     (501) staff       (20)      378 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/MANIFEST.in
--rw-r--r--   0 tienpx     (501) staff       (20)     9898 2024-02-02 09:44:40.833906 flutter_gen-2.1.2/PKG-INFO
--rw-r--r--   0 tienpx     (501) staff       (20)     9859 2023-09-30 11:01:59.000000 flutter_gen-2.1.2/README.md
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.821228 flutter_gen-2.1.2/flutter_gen/
--rw-r--r--   0 tienpx     (501) staff       (20)       23 2024-02-02 09:44:18.000000 flutter_gen-2.1.2/flutter_gen/__init__.py
--rw-r--r--   0 tienpx     (501) staff       (20)     4159 2024-01-01 16:45:16.000000 flutter_gen-2.1.2/flutter_gen/__main__.py
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.822288 flutter_gen-2.1.2/flutter_gen/config/
--rw-r--r--   0 tienpx     (501) staff       (20)     3153 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/config/config_cmd.py
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.823114 flutter_gen-2.1.2/flutter_gen/core/
--rw-r--r--   0 tienpx     (501) staff       (20)      839 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/core/command.py
--rw-r--r--   0 tienpx     (501) staff       (20)     1061 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/core/constants.py
--rw-r--r--   0 tienpx     (501) staff       (20)      104 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/core/model.py
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.823547 flutter_gen-2.1.2/flutter_gen/create/
--rw-r--r--   0 tienpx     (501) staff       (20)      776 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/create/create_cmd.py
--rw-r--r--   0 tienpx     (501) staff       (20)     1084 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/create/create_i18n.py
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.823759 flutter_gen-2.1.2/flutter_gen/figma/
--rw-r--r--   0 tienpx     (501) staff       (20)     1539 2023-09-30 11:01:59.000000 flutter_gen-2.1.2/flutter_gen/figma/generate_text.py
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.826498 flutter_gen-2.1.2/flutter_gen/generate/
--rw-r--r--   0 tienpx     (501) staff       (20)     1169 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/generate/generate_color_cmd.py
--rw-r--r--   0 tienpx     (501) staff       (20)     1572 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/generate/generate_font_cmd.py
--rw-r--r--   0 tienpx     (501) staff       (20)     2122 2024-01-02 16:54:31.000000 flutter_gen-2.1.2/flutter_gen/generate/generate_image_cmd.py
--rw-r--r--   0 tienpx     (501) staff       (20)     2280 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/generate/generate_localization_cmd.py
--rw-r--r--   0 tienpx     (501) staff       (20)     2721 2023-09-30 11:01:59.000000 flutter_gen-2.1.2/flutter_gen/generate/generate_object_freezed_cmd.py
--rw-r--r--   0 tienpx     (501) staff       (20)     2786 2023-09-30 11:01:59.000000 flutter_gen-2.1.2/flutter_gen/generate/generate_object_mapper_cmd.py
--rw-r--r--   0 tienpx     (501) staff       (20)     4560 2024-02-02 09:44:36.000000 flutter_gen-2.1.2/flutter_gen/generate/generate_r_cmd.py
--rw-r--r--   0 tienpx     (501) staff       (20)     2461 2023-10-01 07:03:58.000000 flutter_gen-2.1.2/flutter_gen/generate/generate_repo_cmd.py
--rw-r--r--   0 tienpx     (501) staff       (20)     3010 2023-10-01 07:04:24.000000 flutter_gen-2.1.2/flutter_gen/generate/generate_router_cmd.py
--rw-r--r--   0 tienpx     (501) staff       (20)      889 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/generate/sync_cmd.py
--rw-r--r--   0 tienpx     (501) staff       (20)     5412 2024-01-16 06:20:54.000000 flutter_gen-2.1.2/flutter_gen/generate/watch_cmd.py
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.826652 flutter_gen-2.1.2/flutter_gen/intellji/
--rw-r--r--   0 tienpx     (501) staff       (20)     1096 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/intellji/install_cmd.py
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.827014 flutter_gen-2.1.2/flutter_gen/rename/
--rw-r--r--   0 tienpx     (501) staff       (20)      374 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/rename/config.py
--rw-r--r--   0 tienpx     (501) staff       (20)     1245 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/rename/rename_cmd.py
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.827836 flutter_gen-2.1.2/flutter_gen/template/
--rw-r--r--   0 tienpx     (501) staff       (20)     1479 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/template/api_template.py
--rw-r--r--   0 tienpx     (501) staff       (20)     6267 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/template/base_template.py
--rw-r--r--   0 tienpx     (501) staff       (20)     3169 2024-01-01 16:52:27.000000 flutter_gen-2.1.2/flutter_gen/template/component_cmd.py
--rw-r--r--   0 tienpx     (501) staff       (20)     1353 2024-01-01 16:18:31.000000 flutter_gen-2.1.2/flutter_gen/template/template_cmd.py
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.830070 flutter_gen-2.1.2/flutter_gen/utils/
--rw-r--r--   0 tienpx     (501) staff       (20)     5512 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/utils/dart_helpers.py
--rw-r--r--   0 tienpx     (501) staff       (20)      417 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/utils/debounce.py
--rw-r--r--   0 tienpx     (501) staff       (20)     1633 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/utils/file_helpers.py
--rw-r--r--   0 tienpx     (501) staff       (20)     2570 2023-10-01 06:47:31.000000 flutter_gen-2.1.2/flutter_gen/utils/file_replace.py
--rw-r--r--   0 tienpx     (501) staff       (20)     1820 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/utils/intellij.py
--rw-r--r--   0 tienpx     (501) staff       (20)     1519 2024-01-02 16:28:26.000000 flutter_gen-2.1.2/flutter_gen/utils/json_helpers.py
--rw-r--r--   0 tienpx     (501) staff       (20)     1318 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/utils/loader.py
--rw-r--r--   0 tienpx     (501) staff       (20)      137 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/utils/pb.py
--rw-r--r--   0 tienpx     (501) staff       (20)      730 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/utils/print.py
--rw-r--r--   0 tienpx     (501) staff       (20)     1015 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/utils/str_helpers.py
--rw-r--r--   0 tienpx     (501) staff       (20)     2735 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen/utils/utils.py
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.822150 flutter_gen-2.1.2/flutter_gen.egg-info/
--rw-r--r--   0 tienpx     (501) staff       (20)     9898 2024-02-02 09:44:40.000000 flutter_gen-2.1.2/flutter_gen.egg-info/PKG-INFO
--rw-r--r--   0 tienpx     (501) staff       (20)     2271 2024-02-02 09:44:40.000000 flutter_gen-2.1.2/flutter_gen.egg-info/SOURCES.txt
--rw-r--r--   0 tienpx     (501) staff       (20)        1 2024-02-02 09:44:40.000000 flutter_gen-2.1.2/flutter_gen.egg-info/dependency_links.txt
--rw-r--r--   0 tienpx     (501) staff       (20)       58 2024-02-02 09:44:40.000000 flutter_gen-2.1.2/flutter_gen.egg-info/entry_points.txt
--rw-r--r--   0 tienpx     (501) staff       (20)      122 2024-02-02 09:44:40.000000 flutter_gen-2.1.2/flutter_gen.egg-info/requires.txt
--rw-r--r--   0 tienpx     (501) staff       (20)      207 2024-02-02 09:44:40.000000 flutter_gen-2.1.2/flutter_gen.egg-info/top_level.txt
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.830242 flutter_gen-2.1.2/flutter_gen_templates/
--rw-r--r--   0 tienpx     (501) staff       (20)        0 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen_templates/__init__.py
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.830396 flutter_gen-2.1.2/flutter_gen_templates/api/
--rw-r--r--   0 tienpx     (501) staff       (20)      828 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen_templates/api/api.dart
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.830857 flutter_gen-2.1.2/flutter_gen_templates/base/
--rw-r--r--   0 tienpx     (501) staff       (20)      864 2024-01-07 10:52:43.000000 flutter_gen-2.1.2/flutter_gen_templates/base/view.dart
--rw-r--r--   0 tienpx     (501) staff       (20)      989 2023-09-30 11:01:59.000000 flutter_gen-2.1.2/flutter_gen_templates/base/viewmodel.dart
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.831526 flutter_gen-2.1.2/flutter_gen_templates/commands/
--rw-r--r--   0 tienpx     (501) staff       (20)        0 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen_templates/commands/api.dart
--rw-r--r--   0 tienpx     (501) staff       (20)      688 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen_templates/commands/json.dart
--rw-r--r--   0 tienpx     (501) staff       (20)      729 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen_templates/commands/mock.dart
--rw-r--r--   0 tienpx     (501) staff       (20)      171 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/flutter_gen_templates/commands/to_string.dart
-drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-02-02 09:44:40.833499 flutter_gen-2.1.2/flutter_gen_templates/gen/
--rw-r--r--   0 tienpx     (501) staff       (20)      242 2023-09-30 11:01:59.000000 flutter_gen-2.1.2/flutter_gen_templates/gen/colors.dart
--rw-r--r--   0 tienpx     (501) staff       (20)      164 2024-01-01 16:47:03.000000 flutter_gen-2.1.2/flutter_gen_templates/gen/component.dart
--rw-r--r--   0 tienpx     (501) staff       (20)      390 2023-09-30 11:01:59.000000 flutter_gen-2.1.2/flutter_gen_templates/gen/entities.dart
--rw-r--r--   0 tienpx     (501) staff       (20)      204 2023-09-30 11:01:59.000000 flutter_gen-2.1.2/flutter_gen_templates/gen/fonts.dart
--rw-r--r--   0 tienpx     (501) staff       (20)      524 2023-09-30 11:01:59.000000 flutter_gen-2.1.2/flutter_gen_templates/gen/freezed.dart
--rw-r--r--   0 tienpx     (501) staff       (20)      313 2023-09-30 11:01:59.000000 flutter_gen-2.1.2/flutter_gen_templates/gen/i18n.dart
--rw-r--r--   0 tienpx     (501) staff       (20)     3220 2023-09-30 11:01:59.000000 flutter_gen-2.1.2/flutter_gen_templates/gen/images.dart
--rw-r--r--   0 tienpx     (501) staff       (20)     4206 2024-01-02 16:19:36.000000 flutter_gen-2.1.2/flutter_gen_templates/gen/r.dart
--rw-r--r--   0 tienpx     (501) staff       (20)      420 2023-09-30 11:01:59.000000 flutter_gen-2.1.2/flutter_gen_templates/gen/repository.dart
--rw-r--r--   0 tienpx     (501) staff       (20)     3049 2024-01-02 16:30:41.000000 flutter_gen-2.1.2/flutter_gen_templates/gen/router.dart
--rw-r--r--   0 tienpx     (501) staff       (20)       38 2024-02-02 09:44:40.834157 flutter_gen-2.1.2/setup.cfg
--rw-r--r--   0 tienpx     (501) staff       (20)     1432 2022-05-30 12:39:38.000000 flutter_gen-2.1.2/setup.py
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.204595 flutter_gen-2.2.0/
+-rw-r--r--   0 tienpx     (501) staff       (20)     1092 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/LICENSE
+-rw-r--r--   0 tienpx     (501) staff       (20)      378 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/MANIFEST.in
+-rw-r--r--   0 tienpx     (501) staff       (20)     9898 2024-05-10 03:38:14.204391 flutter_gen-2.2.0/PKG-INFO
+-rw-r--r--   0 tienpx     (501) staff       (20)     9859 2023-09-30 11:01:59.000000 flutter_gen-2.2.0/README.md
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.193243 flutter_gen-2.2.0/flutter_gen/
+-rw-r--r--   0 tienpx     (501) staff       (20)       23 2024-05-10 02:54:16.000000 flutter_gen-2.2.0/flutter_gen/__init__.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     4015 2024-05-10 02:53:13.000000 flutter_gen-2.2.0/flutter_gen/__main__.py
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.194217 flutter_gen-2.2.0/flutter_gen/config/
+-rw-r--r--   0 tienpx     (501) staff       (20)     3153 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/config/config_cmd.py
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.195019 flutter_gen-2.2.0/flutter_gen/core/
+-rw-r--r--   0 tienpx     (501) staff       (20)      839 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/core/command.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     1061 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/core/constants.py
+-rw-r--r--   0 tienpx     (501) staff       (20)      104 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/core/model.py
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.195454 flutter_gen-2.2.0/flutter_gen/create/
+-rw-r--r--   0 tienpx     (501) staff       (20)      776 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/create/create_cmd.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     1084 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/create/create_i18n.py
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.195631 flutter_gen-2.2.0/flutter_gen/figma/
+-rw-r--r--   0 tienpx     (501) staff       (20)     1539 2023-09-30 11:01:59.000000 flutter_gen-2.2.0/flutter_gen/figma/generate_text.py
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.197936 flutter_gen-2.2.0/flutter_gen/generate/
+-rw-r--r--   0 tienpx     (501) staff       (20)     1169 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/generate/generate_color_cmd.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     1572 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/generate/generate_font_cmd.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     2122 2024-01-02 16:54:31.000000 flutter_gen-2.2.0/flutter_gen/generate/generate_image_cmd.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     2280 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/generate/generate_localization_cmd.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     2721 2023-09-30 11:01:59.000000 flutter_gen-2.2.0/flutter_gen/generate/generate_object_freezed_cmd.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     2786 2023-09-30 11:01:59.000000 flutter_gen-2.2.0/flutter_gen/generate/generate_object_mapper_cmd.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     4560 2024-02-02 09:44:36.000000 flutter_gen-2.2.0/flutter_gen/generate/generate_r_cmd.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     2461 2023-10-01 07:03:58.000000 flutter_gen-2.2.0/flutter_gen/generate/generate_repo_cmd.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     3010 2023-10-01 07:04:24.000000 flutter_gen-2.2.0/flutter_gen/generate/generate_router_cmd.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     1840 2024-05-10 03:35:55.000000 flutter_gen-2.2.0/flutter_gen/generate/sync_cmd.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     5412 2024-01-16 06:20:54.000000 flutter_gen-2.2.0/flutter_gen/generate/watch_cmd.py
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.198089 flutter_gen-2.2.0/flutter_gen/intellji/
+-rw-r--r--   0 tienpx     (501) staff       (20)     1096 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/intellji/install_cmd.py
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.198404 flutter_gen-2.2.0/flutter_gen/rename/
+-rw-r--r--   0 tienpx     (501) staff       (20)      374 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/rename/config.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     1245 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/rename/rename_cmd.py
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.199113 flutter_gen-2.2.0/flutter_gen/template/
+-rw-r--r--   0 tienpx     (501) staff       (20)     1479 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/template/api_template.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     6267 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/template/base_template.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     3169 2024-01-01 16:52:27.000000 flutter_gen-2.2.0/flutter_gen/template/component_cmd.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     1353 2024-01-01 16:18:31.000000 flutter_gen-2.2.0/flutter_gen/template/template_cmd.py
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.201108 flutter_gen-2.2.0/flutter_gen/utils/
+-rw-r--r--   0 tienpx     (501) staff       (20)     5512 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/utils/dart_helpers.py
+-rw-r--r--   0 tienpx     (501) staff       (20)      417 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/utils/debounce.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     1633 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/utils/file_helpers.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     2570 2023-10-01 06:47:31.000000 flutter_gen-2.2.0/flutter_gen/utils/file_replace.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     1820 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/utils/intellij.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     1519 2024-01-02 16:28:26.000000 flutter_gen-2.2.0/flutter_gen/utils/json_helpers.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     1318 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/utils/loader.py
+-rw-r--r--   0 tienpx     (501) staff       (20)      137 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/utils/pb.py
+-rw-r--r--   0 tienpx     (501) staff       (20)      730 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/utils/print.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     1015 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/utils/str_helpers.py
+-rw-r--r--   0 tienpx     (501) staff       (20)     2735 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen/utils/utils.py
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.194073 flutter_gen-2.2.0/flutter_gen.egg-info/
+-rw-r--r--   0 tienpx     (501) staff       (20)     9898 2024-05-10 03:38:14.000000 flutter_gen-2.2.0/flutter_gen.egg-info/PKG-INFO
+-rw-r--r--   0 tienpx     (501) staff       (20)     2271 2024-05-10 03:38:14.000000 flutter_gen-2.2.0/flutter_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 tienpx     (501) staff       (20)        1 2024-05-10 03:38:14.000000 flutter_gen-2.2.0/flutter_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 tienpx     (501) staff       (20)       58 2024-05-10 03:38:14.000000 flutter_gen-2.2.0/flutter_gen.egg-info/entry_points.txt
+-rw-r--r--   0 tienpx     (501) staff       (20)      122 2024-05-10 03:38:14.000000 flutter_gen-2.2.0/flutter_gen.egg-info/requires.txt
+-rw-r--r--   0 tienpx     (501) staff       (20)      207 2024-05-10 03:38:14.000000 flutter_gen-2.2.0/flutter_gen.egg-info/top_level.txt
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.201287 flutter_gen-2.2.0/flutter_gen_templates/
+-rw-r--r--   0 tienpx     (501) staff       (20)        0 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen_templates/__init__.py
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.201392 flutter_gen-2.2.0/flutter_gen_templates/api/
+-rw-r--r--   0 tienpx     (501) staff       (20)      828 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen_templates/api/api.dart
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.201773 flutter_gen-2.2.0/flutter_gen_templates/base/
+-rw-r--r--   0 tienpx     (501) staff       (20)      864 2024-01-07 10:52:43.000000 flutter_gen-2.2.0/flutter_gen_templates/base/view.dart
+-rw-r--r--   0 tienpx     (501) staff       (20)      989 2023-09-30 11:01:59.000000 flutter_gen-2.2.0/flutter_gen_templates/base/viewmodel.dart
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.202344 flutter_gen-2.2.0/flutter_gen_templates/commands/
+-rw-r--r--   0 tienpx     (501) staff       (20)        0 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen_templates/commands/api.dart
+-rw-r--r--   0 tienpx     (501) staff       (20)      688 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen_templates/commands/json.dart
+-rw-r--r--   0 tienpx     (501) staff       (20)      729 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen_templates/commands/mock.dart
+-rw-r--r--   0 tienpx     (501) staff       (20)      171 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/flutter_gen_templates/commands/to_string.dart
+drwxr-xr-x   0 tienpx     (501) staff       (20)        0 2024-05-10 03:38:14.204068 flutter_gen-2.2.0/flutter_gen_templates/gen/
+-rw-r--r--   0 tienpx     (501) staff       (20)      242 2023-09-30 11:01:59.000000 flutter_gen-2.2.0/flutter_gen_templates/gen/colors.dart
+-rw-r--r--   0 tienpx     (501) staff       (20)      164 2024-01-01 16:47:03.000000 flutter_gen-2.2.0/flutter_gen_templates/gen/component.dart
+-rw-r--r--   0 tienpx     (501) staff       (20)      390 2023-09-30 11:01:59.000000 flutter_gen-2.2.0/flutter_gen_templates/gen/entities.dart
+-rw-r--r--   0 tienpx     (501) staff       (20)      204 2023-09-30 11:01:59.000000 flutter_gen-2.2.0/flutter_gen_templates/gen/fonts.dart
+-rw-r--r--   0 tienpx     (501) staff       (20)      524 2023-09-30 11:01:59.000000 flutter_gen-2.2.0/flutter_gen_templates/gen/freezed.dart
+-rw-r--r--   0 tienpx     (501) staff       (20)      313 2023-09-30 11:01:59.000000 flutter_gen-2.2.0/flutter_gen_templates/gen/i18n.dart
+-rw-r--r--   0 tienpx     (501) staff       (20)     3220 2023-09-30 11:01:59.000000 flutter_gen-2.2.0/flutter_gen_templates/gen/images.dart
+-rw-r--r--   0 tienpx     (501) staff       (20)     4206 2024-01-02 16:19:36.000000 flutter_gen-2.2.0/flutter_gen_templates/gen/r.dart
+-rw-r--r--   0 tienpx     (501) staff       (20)      420 2023-09-30 11:01:59.000000 flutter_gen-2.2.0/flutter_gen_templates/gen/repository.dart
+-rw-r--r--   0 tienpx     (501) staff       (20)     3049 2024-01-02 16:30:41.000000 flutter_gen-2.2.0/flutter_gen_templates/gen/router.dart
+-rw-r--r--   0 tienpx     (501) staff       (20)       38 2024-05-10 03:38:14.204640 flutter_gen-2.2.0/setup.cfg
+-rw-r--r--   0 tienpx     (501) staff       (20)     1432 2022-05-30 12:39:38.000000 flutter_gen-2.2.0/setup.py
```

### Comparing `flutter_gen-2.1.2/LICENSE` & `flutter_gen-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/PKG-INFO` & `flutter_gen-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flutter_gen
-Version: 2.1.2
+Version: 2.2.0
 Summary: A code generator for Flutter
 Home-page: https://github.com/tien-px/pt_flutter_tools
 Author: Pham Xuan Tien
 Author-email: tienpx.x.x@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `flutter_gen-2.1.2/README.md` & `flutter_gen-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/__main__.py` & `flutter_gen-2.2.0/flutter_gen/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -80,18 +80,15 @@
 def cmd_template(parser, context, args):
     parser.description = ""
     InstallCommand().run()
 
 
 @subcmd("run", help="run")
 def cmd_template(parser, context, args):
-    parser.description = "run"
-    parser.add_argument("path", nargs=1, help="document path")
-    args = parser.parse_args(args)
-    RunCommand(args.path[0]).run()
+    RunCommand().run()
 
 
 def exit_handler():
     Intellij.getInstance().to_file()
 
 
 def main():
```

### Comparing `flutter_gen-2.1.2/flutter_gen/config/config_cmd.py` & `flutter_gen-2.2.0/flutter_gen/config/config_cmd.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/core/command.py` & `flutter_gen-2.2.0/flutter_gen/core/command.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/core/constants.py` & `flutter_gen-2.2.0/flutter_gen/core/constants.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/create/create_cmd.py` & `flutter_gen-2.2.0/flutter_gen/create/create_cmd.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/create/create_i18n.py` & `flutter_gen-2.2.0/flutter_gen/create/create_i18n.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/figma/generate_text.py` & `flutter_gen-2.2.0/flutter_gen/figma/generate_text.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/generate/generate_color_cmd.py` & `flutter_gen-2.2.0/flutter_gen/generate/generate_color_cmd.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/generate/generate_font_cmd.py` & `flutter_gen-2.2.0/flutter_gen/generate/generate_font_cmd.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/generate/generate_image_cmd.py` & `flutter_gen-2.2.0/flutter_gen/generate/generate_image_cmd.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/generate/generate_localization_cmd.py` & `flutter_gen-2.2.0/flutter_gen/generate/generate_localization_cmd.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/generate/generate_object_freezed_cmd.py` & `flutter_gen-2.2.0/flutter_gen/generate/generate_object_freezed_cmd.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/generate/generate_object_mapper_cmd.py` & `flutter_gen-2.2.0/flutter_gen/generate/generate_object_mapper_cmd.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/generate/generate_r_cmd.py` & `flutter_gen-2.2.0/flutter_gen/generate/generate_r_cmd.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/generate/generate_repo_cmd.py` & `flutter_gen-2.2.0/flutter_gen/generate/generate_repo_cmd.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/generate/generate_router_cmd.py` & `flutter_gen-2.2.0/flutter_gen/generate/generate_router_cmd.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/generate/watch_cmd.py` & `flutter_gen-2.2.0/flutter_gen/generate/watch_cmd.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/intellji/install_cmd.py` & `flutter_gen-2.2.0/flutter_gen/intellji/install_cmd.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/rename/rename_cmd.py` & `flutter_gen-2.2.0/flutter_gen/rename/rename_cmd.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/template/api_template.py` & `flutter_gen-2.2.0/flutter_gen/template/api_template.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/template/base_template.py` & `flutter_gen-2.2.0/flutter_gen/template/base_template.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/template/component_cmd.py` & `flutter_gen-2.2.0/flutter_gen/template/component_cmd.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/template/template_cmd.py` & `flutter_gen-2.2.0/flutter_gen/template/template_cmd.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/utils/dart_helpers.py` & `flutter_gen-2.2.0/flutter_gen/utils/dart_helpers.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/utils/file_helpers.py` & `flutter_gen-2.2.0/flutter_gen/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/utils/file_replace.py` & `flutter_gen-2.2.0/flutter_gen/utils/file_replace.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/utils/intellij.py` & `flutter_gen-2.2.0/flutter_gen/utils/intellij.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/utils/json_helpers.py` & `flutter_gen-2.2.0/flutter_gen/utils/json_helpers.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/utils/loader.py` & `flutter_gen-2.2.0/flutter_gen/utils/loader.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/utils/print.py` & `flutter_gen-2.2.0/flutter_gen/utils/print.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/utils/str_helpers.py` & `flutter_gen-2.2.0/flutter_gen/utils/str_helpers.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen/utils/utils.py` & `flutter_gen-2.2.0/flutter_gen/utils/utils.py`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen.egg-info/PKG-INFO` & `flutter_gen-2.2.0/flutter_gen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flutter-gen
-Version: 2.1.2
+Version: 2.2.0
 Summary: A code generator for Flutter
 Home-page: https://github.com/tien-px/pt_flutter_tools
 Author: Pham Xuan Tien
 Author-email: tienpx.x.x@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `flutter_gen-2.1.2/flutter_gen.egg-info/SOURCES.txt` & `flutter_gen-2.2.0/flutter_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen_templates/api/api.dart` & `flutter_gen-2.2.0/flutter_gen_templates/api/api.dart`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen_templates/base/view.dart` & `flutter_gen-2.2.0/flutter_gen_templates/base/view.dart`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen_templates/base/viewmodel.dart` & `flutter_gen-2.2.0/flutter_gen_templates/base/viewmodel.dart`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen_templates/commands/json.dart` & `flutter_gen-2.2.0/flutter_gen_templates/commands/json.dart`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen_templates/commands/mock.dart` & `flutter_gen-2.2.0/flutter_gen_templates/commands/mock.dart`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen_templates/gen/freezed.dart` & `flutter_gen-2.2.0/flutter_gen_templates/gen/freezed.dart`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen_templates/gen/images.dart` & `flutter_gen-2.2.0/flutter_gen_templates/gen/images.dart`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen_templates/gen/r.dart` & `flutter_gen-2.2.0/flutter_gen_templates/gen/r.dart`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/flutter_gen_templates/gen/router.dart` & `flutter_gen-2.2.0/flutter_gen_templates/gen/router.dart`

 * *Files identical despite different names*

### Comparing `flutter_gen-2.1.2/setup.py` & `flutter_gen-2.2.0/setup.py`

 * *Files identical despite different names*

