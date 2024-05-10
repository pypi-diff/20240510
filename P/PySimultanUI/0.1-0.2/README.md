# Comparing `tmp/pysimultanui-0.1.tar.gz` & `tmp/pysimultanui-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysimultanui-0.1.tar", last modified: Mon May  6 20:48:24 2024, max compression
+gzip compressed data, was "pysimultanui-0.2.tar", last modified: Thu May  9 18:49:29 2024, max compression
```

## Comparing `pysimultanui-0.1.tar` & `pysimultanui-0.2.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 20:48:24.667661 pysimultanui-0.1/
--rw-rw-rw-   0        0        0     1023 2020-08-04 12:27:59.000000 pysimultanui-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       93 2024-05-06 20:44:28.000000 pysimultanui-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1774 2024-05-06 20:48:24.667661 pysimultanui-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-05-06 20:43:43.000000 pysimultanui-0.1/README.md
--rw-rw-rw-   0        0        0     1251 2024-05-06 20:44:06.000000 pysimultanui-0.1/pyproject.toml
--rw-rw-rw-   0        0        0      171 2024-05-06 20:42:54.000000 pysimultanui-0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 20:48:24.667661 pysimultanui-0.1/setup.cfg
--rw-rw-rw-   0        0        0     2035 2024-05-06 20:42:23.000000 pysimultanui-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 20:48:24.625514 pysimultanui-0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 20:48:24.666661 pysimultanui-0.1/src/PySimultanUI.egg-info/
--rw-rw-rw-   0        0        0     1774 2024-05-06 20:48:24.000000 pysimultanui-0.1/src/PySimultanUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1511 2024-05-06 20:48:24.000000 pysimultanui-0.1/src/PySimultanUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 20:48:24.000000 pysimultanui-0.1/src/PySimultanUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 20:45:19.000000 pysimultanui-0.1/src/PySimultanUI.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2024-05-06 20:48:24.000000 pysimultanui-0.1/src/PySimultanUI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 20:48:24.641518 pysimultanui-0.1/src/app/
--rw-rw-rw-   0        0        0        2 2024-04-22 04:37:47.000000 pysimultanui-0.1/src/app/__init__.py
--rw-rw-rw-   0        0        0      856 2024-04-12 08:27:14.000000 pysimultanui-0.1/src/app/auth.py
--rw-rw-rw-   0        0        0      390 2024-05-05 17:27:11.000000 pysimultanui-0.1/src/app/home.py
--rw-rw-rw-   0        0        0     1412 2024-04-23 06:26:45.000000 pysimultanui-0.1/src/app/login.py
--rw-rw-rw-   0        0        0      111 2024-04-12 13:12:18.000000 pysimultanui-0.1/src/app/menue.py
--rw-rw-rw-   0        0        0      304 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/app/project.py
--rw-rw-rw-   0        0        0     3151 2024-05-05 17:27:07.000000 pysimultanui-0.1/src/app/theme.py
-drwxrwxrwx   0        0        0        0 2024-05-06 20:48:24.647082 pysimultanui-0.1/src/core/
--rw-rw-rw-   0        0        0      986 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/core/__init__.py
--rw-rw-rw-   0        0        0    14145 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/core/edit_dialog.py
-drwxrwxrwx   0        0        0        0 2024-05-06 20:48:24.648081 pysimultanui-0.1/src/core/freecad_utils/
--rw-rw-rw-   0        0        0        0 2024-04-21 04:11:30.000000 pysimultanui-0.1/src/core/freecad_utils/__init__.py
--rw-rw-rw-   0        0        0     5671 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/core/freecad_utils/tools.py
--rw-rw-rw-   0        0        0      592 2024-05-02 11:33:48.000000 pysimultanui-0.1/src/core/logging.py
--rw-rw-rw-   0        0        0     7423 2024-05-05 17:55:03.000000 pysimultanui-0.1/src/core/method_mapper.py
--rw-rw-rw-   0        0        0     2597 2024-05-06 04:28:48.000000 pysimultanui-0.1/src/core/navigation.py
--rw-rw-rw-   0        0        0    23083 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/core/project_manager.py
--rw-rw-rw-   0        0        0      591 2024-04-16 05:37:02.000000 pysimultanui-0.1/src/core/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-06 20:48:24.653082 pysimultanui-0.1/src/views/
--rw-rw-rw-   0        0        0        0 2024-04-23 06:11:01.000000 pysimultanui-0.1/src/views/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 20:48:24.655083 pysimultanui-0.1/src/views/asset_view/
--rw-rw-rw-   0        0        0       76 2024-04-23 12:28:24.000000 pysimultanui-0.1/src/views/asset_view/__init__.py
--rw-rw-rw-   0        0        0     2132 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/views/asset_view/asset_manager.py
--rw-rw-rw-   0        0        0     1068 2024-05-03 04:04:56.000000 pysimultanui-0.1/src/views/asset_view/asset_view.py
-drwxrwxrwx   0        0        0        0 2024-05-06 20:48:24.657083 pysimultanui-0.1/src/views/component_dict_view/
--rw-rw-rw-   0        0        0      110 2024-04-29 18:57:03.000000 pysimultanui-0.1/src/views/component_dict_view/__init__.py
--rw-rw-rw-   0        0        0      716 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/views/component_dict_view/component_dict_manager.py
--rw-rw-rw-   0        0        0     7183 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/views/component_dict_view/component_dict_view.py
-drwxrwxrwx   0        0        0        0 2024-05-06 20:48:24.659657 pysimultanui-0.1/src/views/component_list_view/
--rw-rw-rw-   0        0        0        0 2024-04-25 05:01:23.000000 pysimultanui-0.1/src/views/component_list_view/__init__.py
--rw-rw-rw-   0        0        0      704 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/views/component_list_view/component_list_manager.py
--rw-rw-rw-   0        0        0     8442 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/views/component_list_view/component_list_view.py
-drwxrwxrwx   0        0        0        0 2024-05-06 20:48:24.662662 pysimultanui-0.1/src/views/geometry_view/
--rw-rw-rw-   0        0        0       88 2024-04-23 12:23:28.000000 pysimultanui-0.1/src/views/geometry_view/__init__.py
--rw-rw-rw-   0        0        0     6578 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/views/geometry_view/geometry_manager.py
--rw-rw-rw-   0        0        0     6410 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/views/geometry_view/geometry_view.py
--rw-rw-rw-   0        0        0     2834 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/views/geometry_view/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-06 20:48:24.664661 pysimultanui-0.1/src/views/mapped_cls/
--rw-rw-rw-   0        0        0       49 2024-04-24 18:10:16.000000 pysimultanui-0.1/src/views/mapped_cls/__init__.py
--rw-rw-rw-   0        0        0     2827 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/views/mapped_cls/mapped_cls_manager.py
--rw-rw-rw-   0        0        0     9493 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/views/mapped_cls/mapped_cls_view.py
--rw-rw-rw-   0        0        0     6679 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/views/numpy_view.py
--rw-rw-rw-   0        0        0     4879 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/views/pandas_df_view.py
--rw-rw-rw-   0        0        0     2230 2024-05-02 20:05:22.000000 pysimultanui-0.1/src/views/parameter_view.py
--rw-rw-rw-   0        0        0     3030 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/views/type_view.py
--rw-rw-rw-   0        0        0     6401 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/views/type_view_manager.py
--rw-rw-rw-   0        0        0     5722 2024-05-06 20:48:16.000000 pysimultanui-0.1/src/views/view_manager.py
-drwxrwxrwx   0        0        0        0 2024-05-06 20:48:24.665661 pysimultanui-0.1/tests/
--rw-rw-rw-   0        0        0    30468 2024-05-06 20:48:16.000000 pysimultanui-0.1/tests/test_py_simultan_ui.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:49:29.610846 pysimultanui-0.2/
+-rw-rw-rw-   0        0        0     1040 2024-05-09 17:27:15.000000 pysimultanui-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       97 2024-05-09 17:27:15.000000 pysimultanui-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1774 2024-05-09 18:49:29.607580 pysimultanui-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2024-05-09 17:27:15.000000 pysimultanui-0.2/README.md
+-rw-rw-rw-   0        0        0     1309 2024-05-09 18:49:17.000000 pysimultanui-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      189 2024-05-09 17:27:15.000000 pysimultanui-0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 18:49:29.610913 pysimultanui-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2087 2024-05-09 18:49:19.000000 pysimultanui-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:49:29.538316 pysimultanui-0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 18:49:29.606481 pysimultanui-0.2/src/PySimultanUI.egg-info/
+-rw-rw-rw-   0        0        0     1774 2024-05-09 18:49:29.000000 pysimultanui-0.2/src/PySimultanUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1554 2024-05-09 18:49:29.000000 pysimultanui-0.2/src/PySimultanUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 18:49:29.000000 pysimultanui-0.2/src/PySimultanUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-09 18:48:30.000000 pysimultanui-0.2/src/PySimultanUI.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2024-05-09 18:49:29.000000 pysimultanui-0.2/src/PySimultanUI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 18:49:29.563022 pysimultanui-0.2/src/app/
+-rw-rw-rw-   0        0        0        2 2024-04-27 13:04:42.000000 pysimultanui-0.2/src/app/__init__.py
+-rw-rw-rw-   0        0        0      856 2024-04-27 13:04:42.000000 pysimultanui-0.2/src/app/auth.py
+-rw-rw-rw-   0        0        0      557 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/app/home.py
+-rw-rw-rw-   0        0        0     1190 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/app/login.py
+-rw-rw-rw-   0        0        0      111 2024-04-27 13:04:42.000000 pysimultanui-0.2/src/app/menue.py
+-rw-rw-rw-   0        0        0      304 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/app/project.py
+-rw-rw-rw-   0        0        0     3490 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/app/theme.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:49:29.572589 pysimultanui-0.2/src/core/
+-rw-rw-rw-   0        0        0     1042 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/core/__init__.py
+-rw-rw-rw-   0        0        0    14327 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/core/edit_dialog.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:49:29.573945 pysimultanui-0.2/src/core/freecad_utils/
+-rw-rw-rw-   0        0        0        0 2024-04-27 13:04:42.000000 pysimultanui-0.2/src/core/freecad_utils/__init__.py
+-rw-rw-rw-   0        0        0     5671 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/core/freecad_utils/tools.py
+-rw-rw-rw-   0        0        0       61 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/core/logging.py
+-rw-rw-rw-   0        0        0     7740 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/core/method_mapper.py
+-rw-rw-rw-   0        0        0     3080 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/core/navigation.py
+-rw-rw-rw-   0        0        0    22200 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/core/project_manager.py
+-rw-rw-rw-   0        0        0      591 2024-04-27 13:04:42.000000 pysimultanui-0.2/src/core/tools.py
+-rw-rw-rw-   0        0        0     5760 2024-05-09 18:47:27.000000 pysimultanui-0.2/src/core/user.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:49:29.583372 pysimultanui-0.2/src/views/
+-rw-rw-rw-   0        0        0      196 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/views/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:49:29.586983 pysimultanui-0.2/src/views/asset_view/
+-rw-rw-rw-   0        0        0       76 2024-04-27 13:04:42.000000 pysimultanui-0.2/src/views/asset_view/__init__.py
+-rw-rw-rw-   0        0        0     1991 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/views/asset_view/asset_manager.py
+-rw-rw-rw-   0        0        0     1068 2024-05-05 18:09:42.000000 pysimultanui-0.2/src/views/asset_view/asset_view.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:49:29.591373 pysimultanui-0.2/src/views/component_dict_view/
+-rw-rw-rw-   0        0        0      110 2024-05-05 18:09:42.000000 pysimultanui-0.2/src/views/component_dict_view/__init__.py
+-rw-rw-rw-   0        0        0      716 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/views/component_dict_view/component_dict_manager.py
+-rw-rw-rw-   0        0        0     7492 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/views/component_dict_view/component_dict_view.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:49:29.595866 pysimultanui-0.2/src/views/component_list_view/
+-rw-rw-rw-   0        0        0        0 2024-04-27 13:04:42.000000 pysimultanui-0.2/src/views/component_list_view/__init__.py
+-rw-rw-rw-   0        0        0      704 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/views/component_list_view/component_list_manager.py
+-rw-rw-rw-   0        0        0     9953 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/views/component_list_view/component_list_view.py
+-rw-rw-rw-   0        0        0     3330 2024-05-09 18:36:55.000000 pysimultanui-0.2/src/views/detail_views.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:49:29.600146 pysimultanui-0.2/src/views/geometry_view/
+-rw-rw-rw-   0        0        0       88 2024-04-27 13:04:42.000000 pysimultanui-0.2/src/views/geometry_view/__init__.py
+-rw-rw-rw-   0        0        0     6222 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/views/geometry_view/geometry_manager.py
+-rw-rw-rw-   0        0        0     6361 2024-05-09 17:45:30.000000 pysimultanui-0.2/src/views/geometry_view/geometry_view.py
+-rw-rw-rw-   0        0        0     2834 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/views/geometry_view/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:49:29.603258 pysimultanui-0.2/src/views/mapped_cls/
+-rw-rw-rw-   0        0        0       49 2024-04-27 13:04:42.000000 pysimultanui-0.2/src/views/mapped_cls/__init__.py
+-rw-rw-rw-   0        0        0     2825 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/views/mapped_cls/mapped_cls_manager.py
+-rw-rw-rw-   0        0        0    10882 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/views/mapped_cls/mapped_cls_view.py
+-rw-rw-rw-   0        0        0     6503 2024-05-09 17:45:07.000000 pysimultanui-0.2/src/views/numpy_view.py
+-rw-rw-rw-   0        0        0     6952 2024-05-09 17:44:27.000000 pysimultanui-0.2/src/views/pandas_df_view.py
+-rw-rw-rw-   0        0        0     2230 2024-05-05 18:09:42.000000 pysimultanui-0.2/src/views/parameter_view.py
+-rw-rw-rw-   0        0        0     2403 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/views/type_view.py
+-rw-rw-rw-   0        0        0     7623 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/views/type_view_manager.py
+-rw-rw-rw-   0        0        0     7036 2024-05-09 17:27:15.000000 pysimultanui-0.2/src/views/view_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:49:29.604397 pysimultanui-0.2/tests/
+-rw-rw-rw-   0        0        0    30468 2024-05-09 17:27:15.000000 pysimultanui-0.2/tests/test_py_simultan_ui.py
```

### Comparing `pysimultanui-0.1/LICENSE.txt` & `pysimultanui-0.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to
-deal in the Software without restriction, including without limitation the
-rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
-sell copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
-IN THE SOFTWARE.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to
+deal in the Software without restriction, including without limitation the
+rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
+sell copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
+IN THE SOFTWARE.
```

### Comparing `pysimultanui-0.1/PKG-INFO` & `pysimultanui-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySimultanUI
-Version: 0.1
+Version: 0.2
 Home-page: 
 Author: Max Buehler
 Author-email: Max Bühler <maximilian.buehler@tuwien.ac.at>
 License: Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to
         deal in the Software without restriction, including without limitation the
         rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
```

### Comparing `pysimultanui-0.1/pyproject.toml` & `pysimultanui-0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-[project]
-name = "PySimultanUI"
-version = "0.1"
-authors = [
-    {name = "Max Bühler", email = "maximilian.buehler@tuwien.ac.at"}
-]
-readme = "README.md"
-requires-python = ">=3.8"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent"
-]
-license = {file = "LICENSE.txt"}
-
-[build-system]
-requires = ["setuptools", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[tool.setuptools.packages.find]
-where = ["src"]
-
-[tool.black]
-# Use the more relaxed max line length permitted in PEP8.
-line-length = 99
-target-version = ["py38", "py39", "py310", "py311", "py312"]
-exclude = '''
-/(
-    \.eggs
-  | \.git
-  | \.mypy_cache
-  | \.tox
-  | \venv
-  | build
-  | dist
-  | htmlcov
-)/
-'''
-
-[tool.isort]
-profile = "black"
-line_length = 99
-force_sort_within_sections = true
-src_paths = ["docs", "src", "tests", "setup.py"]
-
-[tool.coverage.run]
-branch = true
-
-[tool.coverage.paths]
-# Files with these prefixes are treated as identical for the purposes of coverage combine.
-source = [
-    # The first path is the name to which all paths get unified
-    "src/",
-    # tox on Linux
-    ".tox/py*/lib/python*/site-packages/",
-    # tox on Windows
-    ".tox/py*/Lib/site-packages/",
-]
+[project]
+name = "PySimultanUI"
+version = "0.2"
+authors = [
+    {name = "Max Bühler", email = "maximilian.buehler@tuwien.ac.at"}
+]
+readme = "README.md"
+requires-python = ">=3.8"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent"
+]
+license = {file = "LICENSE.txt"}
+
+[build-system]
+requires = ["setuptools", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.black]
+# Use the more relaxed max line length permitted in PEP8.
+line-length = 99
+target-version = ["py38", "py39", "py310", "py311", "py312"]
+exclude = '''
+/(
+    \.eggs
+  | \.git
+  | \.mypy_cache
+  | \.tox
+  | \venv
+  | build
+  | dist
+  | htmlcov
+)/
+'''
+
+[tool.isort]
+profile = "black"
+line_length = 99
+force_sort_within_sections = true
+src_paths = ["docs", "src", "tests", "setup.py"]
+
+[tool.coverage.run]
+branch = true
+
+[tool.coverage.paths]
+# Files with these prefixes are treated as identical for the purposes of coverage combine.
+source = [
+    # The first path is the name to which all paths get unified
+    "src/",
+    # tox on Linux
+    ".tox/py*/lib/python*/site-packages/",
+    # tox on Windows
+    ".tox/py*/Lib/site-packages/",
+]
```

### Comparing `pysimultanui-0.1/setup.py` & `pysimultanui-0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-#!/usr/bin/env python3
-
-from pathlib import Path
-
-import setuptools
-
-project_dir = Path(__file__).parent
-
-setuptools.setup(
-    name="PySimultanUI",
-    version="0.1",
-    description="UI for PySimultan",
-    # Allow UTF-8 characters in README with encoding argument.
-    long_description=project_dir.joinpath("README.md").read_text(encoding="utf-8"),
-    keywords=["python"],
-    author="Max Buehler",
-    url="",
-    packages=setuptools.find_packages("src"),
-    package_dir={"": "src"},
-    package_data={
-            # This assumes your package is named "your_package_name"
-            "PySimultanUI": ["tests/*"]
-        },
-    # pip 9.0+ will inspect this field when installing to help users install a
-    # compatible version of the library for their Python version.
-    python_requires=">=3.10",
-    setup_requires=["wheel"],
-    # There are some peculiarities on how to include package data for source
-    # distributions using setuptools. You also need to add entries for package
-    # data to MANIFEST.in.
-    # See https://stackoverflow.com/questions/7522250/
-    include_package_data=True,
-    # This is a trick to avoid duplicating dependencies between both setup.py and
-    # requirements.txt.
-    # requirements.txt must be included in MANIFEST.in for this to work.
-    # It does not work for all types of dependencies (e.g. VCS dependencies).
-    # For VCS dependencies, use pip >= 19 and the PEP 508 syntax.
-    #   Example: 'requests @ git+https://github.com/requests/requests.git@branch_or_tag'
-    #   See: https://github.com/pypa/pip/issues/6162
-    install_requires=project_dir.joinpath("requirements.txt").read_text().split("\n"),
-    zip_safe=False,
-    license="MIT",
-    license_files=["LICENSE.txt"],
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3 :: Only",
-    ],
-)
+#!/usr/bin/env python3
+
+from pathlib import Path
+
+import setuptools
+
+project_dir = Path(__file__).parent
+
+setuptools.setup(
+    name="PySimultanUI",
+    version="0.2",
+    description="UI for PySimultan",
+    # Allow UTF-8 characters in README with encoding argument.
+    long_description=project_dir.joinpath("README.md").read_text(encoding="utf-8"),
+    keywords=["python"],
+    author="Max Buehler",
+    url="",
+    packages=setuptools.find_packages("src"),
+    package_dir={"": "src"},
+    package_data={
+            # This assumes your package is named "your_package_name"
+            "PySimultanUI": ["tests/*"]
+        },
+    # pip 9.0+ will inspect this field when installing to help users install a
+    # compatible version of the library for their Python version.
+    python_requires=">=3.10",
+    setup_requires=["wheel"],
+    # There are some peculiarities on how to include package data for source
+    # distributions using setuptools. You also need to add entries for package
+    # data to MANIFEST.in.
+    # See https://stackoverflow.com/questions/7522250/
+    include_package_data=True,
+    # This is a trick to avoid duplicating dependencies between both setup.py and
+    # requirements.txt.
+    # requirements.txt must be included in MANIFEST.in for this to work.
+    # It does not work for all types of dependencies (e.g. VCS dependencies).
+    # For VCS dependencies, use pip >= 19 and the PEP 508 syntax.
+    #   Example: 'requests @ git+https://github.com/requests/requests.git@branch_or_tag'
+    #   See: https://github.com/pypa/pip/issues/6162
+    install_requires=project_dir.joinpath("requirements.txt").read_text().split("\n"),
+    zip_safe=False,
+    license="MIT",
+    license_files=["LICENSE.txt"],
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+    ],
+)
```

### Comparing `pysimultanui-0.1/src/PySimultanUI.egg-info/PKG-INFO` & `pysimultanui-0.2/src/PySimultanUI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySimultanUI
-Version: 0.1
+Version: 0.2
 Home-page: 
 Author: Max Buehler
 Author-email: Max Bühler <maximilian.buehler@tuwien.ac.at>
 License: Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to
         deal in the Software without restriction, including without limitation the
         rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
```

### Comparing `pysimultanui-0.1/src/PySimultanUI.egg-info/SOURCES.txt` & `pysimultanui-0.2/src/PySimultanUI.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,19 @@
 src/core/__init__.py
 src/core/edit_dialog.py
 src/core/logging.py
 src/core/method_mapper.py
 src/core/navigation.py
 src/core/project_manager.py
 src/core/tools.py
+src/core/user.py
 src/core/freecad_utils/__init__.py
 src/core/freecad_utils/tools.py
 src/views/__init__.py
+src/views/detail_views.py
 src/views/numpy_view.py
 src/views/pandas_df_view.py
 src/views/parameter_view.py
 src/views/type_view.py
 src/views/type_view_manager.py
 src/views/view_manager.py
 src/views/asset_view/__init__.py
```

### Comparing `pysimultanui-0.1/src/app/auth.py` & `pysimultanui-0.2/src/app/auth.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.1/src/app/login.py` & `pysimultanui-0.2/src/app/login.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 from nicegui import Client, app, ui
 # from .theme import frame
 # from ..router import router
 from typing import Optional
 from fastapi.responses import RedirectResponse
 
-passwords = {'user1': 'pass1', 'user2': 'pass2',
-             'joerg.wolf@a1.digital': 'Ko<j9564Doash55',
-             'markus.frank@a1.digital': 'OrL6}=hi5-f2'}
+from .. import user_manager
 
 
 def content() -> Optional[RedirectResponse]:
     def try_login() -> None:  # local function to avoid passing username and password as arguments
-        if passwords.get(username.value) == password.value:
+        if user_manager.authenticate(username.value, password.value):
             app.storage.user.update({'username': username.value, 'authenticated': True})
             ui.open(app.storage.user.get('referrer_path', '/'))  # go back to where the user wanted to go
         else:
             ui.notify('Wrong username or password', color='negative')
 
     if app.storage.user.get('authenticated', False):
         return RedirectResponse('/')
     with ui.card().classes('h-full w-full').style('align-items: center;'):
-        ui.image('web_ui/src/static_files/A1_Digital_identifier_pos_RGB.png').classes('w-1/6')
         ui.label('PySimultan WebUI')
         with ui.card():
             username = ui.input('Username').on('keydown.enter', try_login)
             password = ui.input('Password', password=True, password_toggle_button=True).on('keydown.enter', try_login)
             ui.button('Log in', on_click=try_login)
```

### Comparing `pysimultanui-0.1/src/app/theme.py` & `pysimultanui-0.2/src/app/theme.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 from contextlib import contextmanager
 from .menue import menu
 from nicegui import app, ui, context
+from .. import user_manager
 
 from . import home
 from . import project
 
 from .. import core
 
 
 @contextmanager
 def frame(navtitle: str):
 
     """Custom page frame to share the same styling and behavior across all pages"""
     # ui.colors(primary='#da291c', secondary='#941c13', accent='#941c13', positive='#53B689')
-    with ui.header().classes('justify-between h-20'):
+    with ui.header().classes('justify-between h-25'):
+
+        user = user_manager.users[app.storage.user['username']]
 
         # ui.image('web_ui/src/static_files/A1_Digital_identifier_pos_RGB.png').classes('w-32')
 
-        ui.label('PY Simultan').classes('font-bold text-white text-xl')
+        with ui.column():
+            ui.label('PY Simultan').classes('font-bold text-white text-xl')
+            ui.button(on_click=lambda: (app.storage.user.clear(), ui.navigate.to('/login')), icon='logout')
+
+        with ui.column():
+            ui.label(f'Hello {user.name}').classes('text-white text-xl')
 
         # with ui.expansion('Menu', icon='select'):
         with ui.column():
             with ui.tabs() as tabs:
                 ui.button('Mapped Classes', icon='checklist_rtl', on_click=lambda: left_drawer.toggle())
                 ui.tab('Home', icon='home')
                 ui.tab('Project', icon='edit')
@@ -43,15 +51,15 @@
                 #     ui.label(f'{app.storage.user["username"]}').classes('mr-auto text-2xl')
 
     with ui.left_drawer(bordered=True,
                         top_corner=False,
                         elevated=True,
                         fixed=True,
                         value=False).classes('bg-blue-100') as left_drawer:
-        core.navigation_drawer = left_drawer
+        user.navigation_drawer = left_drawer
 
     # with ui.splitter() as splitter:
     #     with splitter.after:
     #         with ui.right_drawer(bordered=True,
     #                              top_corner=False,
     #                              elevated=True,
     #                              fixed=True,
@@ -60,15 +68,15 @@
     #                 core.detail_view = detail_view
 
     with ui.tab_panels(tabs, value='Home').classes('w-full h-full'):
         with ui.tab_panel('Project').classes('w-full h-full') as project_full_tab:
             with ui.splitter(value=60, limits=(10, 90)).classes('w-full h-full') as splitter:
                 with splitter.before:
                     context.client.content.classes('h-[95vh]')
-                    core.project_tab = ui.scroll_area().classes('w-full h-full')
+                    user.project_tab = ui.scroll_area().classes('w-full h-full')
                 with splitter.after:
-                    core.detail_view = ui.card().classes('w-full h-full')
+                    user.detail_view = ui.card().classes('w-full h-full')
 
-        core.home_tab = ui.tab_panel('Home').classes('w-full h-full')
+        user.home_tab = ui.tab_panel('Home').classes('w-full h-full')
 
-    with core.home_tab:
+    with user.home_tab:
         home.content()
```

### Comparing `pysimultanui-0.1/src/core/__init__.py` & `pysimultanui-0.2/src/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from typing import Union
+from .user import UserManager
+
 from PySimultan2.object_mapper import PythonMapper
 from PySimultan2.data_model import DataModel
 from .method_mapper import method_mapper, mapped_method
 from .logging import logger
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
@@ -12,18 +14,19 @@
     from .navigation import Navigation
     from ..views.asset_view import AssetManager
 
 
 mapper = PythonMapper()
 method_mapper.mapper = mapper
 mapper.method_mapper = method_mapper
-data_model: Union[DataModel, None] = None
-navigation: Union['Navigation', None] = None
-view_manager: Union['ViewManager', None] = None
-project_manager: Union['ProjectManager', None] = None
-asset_manager: Union['AssetManager', None] = None
-geometry_manager: Union['GeometryManager', None] = None
 
-navigation_drawer = None
-project_tab = None
-detail_view = None
-home_tab = None
+# data_model: Union[DataModel, None] = None
+# navigation: Union['Navigation', None] = None
+# view_manager: Union['ViewManager', None] = None
+# project_manager: Union['ProjectManager', None] = None
+# asset_manager: Union['AssetManager', None] = None
+# geometry_manager: Union['GeometryManager', None] = None
+#
+# navigation_drawer = None
+# project_tab = None
+# detail_view = None
+# home_tab = None
```

### Comparing `pysimultanui-0.1/src/core/edit_dialog.py` & `pysimultanui-0.2/src/core/edit_dialog.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from nicegui import ui
+from nicegui import ui, app
 
+from .. import user_manager
 from .. import core
 from PySimultan2.simultan_object import SimultanObject
 from PySimultan2.files import FileInfo
 from ..config import logger
 from math import inf
 
 
@@ -132,16 +133,16 @@
             return self.component_name_map[self.component_select.value[0]]
         else:
             return [self.component_name_map[x] for x in self.component_select.value]
 
     def ui_content(self):
         with ui.card():
             ui.label('Select component')
-
-            classes = core.mapper.registered_classes
+            mapper = user_manager[app.storage.user['username']].mapper
+            classes = mapper.registered_classes
 
             if isinstance(self.component, SimultanObject):
                 select_value = self.component._taxonomy
             else:
                 select_value = 'All'
 
             self.class_select = ui.select(['All', *classes.keys()],
@@ -155,19 +156,21 @@
 
     @ui.refreshable
     def component_ui_content(self):
 
         components = []
         self.component_name_map = {}
 
+        mapper = user_manager[app.storage.user['username']].mapper
+
         if 'All' in self.class_select.value:
-            for cls in core.mapper.mapped_classes.values():
+            for cls in mapper.mapped_classes.values():
                 components.extend(cls.cls_instances)
         else:
-            for cls in [core.mapper.get_mapped_class(x) for x in self.class_select.value]:
+            for cls in [mapper.get_mapped_class(x) for x in self.class_select.value]:
                 components.extend(cls.cls_instances)
 
         for component in components:
             self.component_name_map[f'{component.name} ({component.id})'] = component
 
         if isinstance(self.component, SimultanObject):
             select_value = [f'{self.component.name} ({self.component.id})']
@@ -203,18 +206,16 @@
         self.dialog = None
 
         self.asset_name_map = {}
 
     def ui_content(self):
         with ui.card():
             ui.label('Select asset')
-            assets = core.asset_manager.items
-
+            assets = user_manager[app.storage.user['username']].asset_manager.items
             self.asset_name_map = {x.name: x for x in assets}
-
             self.asset_select = ui.select([x.name for x in assets],
                                           label='Select asset',
                                           value=self.asset.name if self.asset is not None else None,
                                           on_change=self.asset_select,
                                           with_input=True
                                           ).classes('w-64').props('use-chips')
 
@@ -340,15 +341,15 @@
             setattr(self.raw_val, 'ValueMin', self.edit_dialog.min)
             setattr(self.raw_val, 'ValueMax', self.edit_dialog.max)
             setattr(self.raw_val, 'Unit', self.edit_dialog.unit)
 
         logger.info(f'Updated {self.content.name} to {self.edit_dialog.value}')
 
         if self.parent is not None:
-            self.parent.ui_content.refresh()
+            self.parent.refresh()
         self.close()
 
 
 class DictEditDialog(object):
 
     def __init__(self, *args, **kwargs):
         self.component = kwargs.get('component', None)
```

### Comparing `pysimultanui-0.1/src/core/freecad_utils/tools.py` & `pysimultanui-0.2/src/core/freecad_utils/tools.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.1/src/core/method_mapper.py` & `pysimultanui-0.2/src/core/method_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import asyncio
 from ..config import logger
-from .. import core
-from nicegui import ui, run
+from nicegui import ui, run, app
 from .tools import ConfirmationDialog
 
 
 class UnknownClass(object):
     def __init__(self, *args, **kwargs):
         self.cls_name: type = kwargs.get('cls_name', 'Unknown class')
         self.cls: type = kwargs.get('cls', None)
@@ -25,15 +24,17 @@
             with ui.item_section():
                 ui.label(self.name)
             with ui.item_section():
                 ui.button(on_click=self.run, icon='play_circle').classes('q-ml-auto')
 
     async def run(self, *args, **kwargs):
 
-        if core.project_manager.data_model is None:
+        from .. import user_manager
+
+        if user_manager[app.storage.user['username']].data_model is None:
             ui.notify('No project loaded!', type='negative')
             return
 
         n = ui.notification(timeout=None)
         n.spinner = True
         n.message = f'Running method {self.name}'
         try:
@@ -64,15 +65,17 @@
             with ui.item_section():
                 ui.label(self.name)
             with ui.item_section():
                 ui.button(on_click=self.run, icon='play_circle').classes('q-ml-auto')
 
     async def run(self, *args, **kwargs):
 
-        if core.project_manager.data_model is None:
+        from .. import user_manager
+
+        if user_manager[app.storage.user['username']].data_model is None:
             ui.notify('No project loaded!', type='negative')
             return
 
         selected_instances = [instance for instance in self.cls.cls_instances if instance.__ui_element__.selected]
         if not selected_instances:
             ui.notify('No instances selected!')
             return
@@ -91,18 +94,23 @@
         if result == 'Yes':
             n = ui.notification(timeout=None)
             n.spinner = True
             n.message = f'Running method {self.name} of {self.cls.__name__}'
             logger.info(f'Running method {self.name} of {self.cls.__name__}')
             await asyncio.sleep(0.01)
             for instance in selected_instances:
-                await run.io_bound(self.method, instance, *args, **kwargs)
+                try:
+                    await run.io_bound(self.method, instance, *args, **kwargs)
                 #
                 # self.method(instance, *self.args, **self.kwargs)
-                instance.__ui_element__.ui_content.refresh()
+                    instance.__ui_element__.ui_content.refresh()
+                except Exception as e:
+                    ui.notify(f'Error running method {self.name} on {instance.name}: {e}', type='negative')
+                    continue
+
                 # getattr(instance, self.name)(*self.args, **self.kwargs)
                 # self.method(instance, *self.args, **self.kwargs)
             ui.notify(f'Method {self.name} run on {len(selected_instances)} instances!')
             n.message = 'Done!'
             n.spinner = False
             await asyncio.sleep(1)
             # self.method(*args, **kwargs)
```

### Comparing `pysimultanui-0.1/src/core/navigation.py` & `pysimultanui-0.2/src/core/navigation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 from typing import Optional, Type
-from nicegui import ui
+from nicegui import ui, app
 
+from .. import user_manager
 from ..import core
 from ..views.type_view_manager import TypeViewManager
 from ..views.view_manager import ViewManager
 
 
 class Navigation(object):
+
     def __init__(self, *args, **kwargs):
+        pass
+        # self._view_manager = None
+        # self.data_model = kwargs.get('data_model', core.data_model)
+        # self.navigation_drawer = core.navigation_drawer
+        # self.view_manager: Optional[Type[ViewManager]] = kwargs.get('view_manager', core.view_manager)
+        # self.geometry_manager: Optional[Type[TypeViewManager]] = kwargs.get('geometry_manager', core.geometry_manager)
+        # self.asset_manager: Type[TypeViewManager] = kwargs.get('asset_manager')
 
-        self._view_manager = None
+    @property
+    def data_model(self):
+        return user_manager[app.storage.user['username']].data_model
 
-        self.data_model = kwargs.get('data_model', core.data_model)
-        self.navigation_drawer = core.navigation_drawer
-        self.view_manager: Optional[Type[ViewManager]] = kwargs.get('view_manager', core.view_manager)
-        self.geometry_manager: Optional[Type[TypeViewManager]] = kwargs.get('geometry_manager', core.geometry_manager)
-        self.asset_manager: Type[TypeViewManager] = kwargs.get('asset_manager')
+    @property
+    def navigation_drawer(self):
+        return user_manager[app.storage.user['username']].navigation_drawer
 
     @property
     def view_manager(self):
-        return self._view_manager
+        return user_manager[app.storage.user['username']].view_manager
 
-    @view_manager.setter
-    def view_manager(self, value):
-        self._view_manager = value
+    @property
+    def geometry_manager(self):
+        return user_manager[app.storage.user['username']].geometry_manager
+
+    @property
+    def asset_manager(self):
+        return user_manager[app.storage.user['username']].asset_manager
 
     @property
     def obj_mapper(self) -> core.PythonMapper:
         return self.view_manager.mapper
 
     @ui.refreshable
     def ui_content(self):
```

### Comparing `pysimultanui-0.1/src/core/project_manager.py` & `pysimultanui-0.2/src/core/project_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import os
 import asyncio
 from copy import deepcopy
+from logging import getLogger
 from typing import Optional, Type
 from datetime import datetime
 from nicegui import app, ui, events
 from PySimultan2.data_model import DataModel
 from PySimultan2.object_mapper import PythonMapper
 from PySimultan2.files import FileInfo
 from PySimultan2.geometry.geometry_base import GeometryModel
 from PySimultan2 import config as py_simultan_config
 
+from .. import user_manager
 from .. import core
+from ..core.user import UserManager, User
 from ..views.view_manager import ViewManager
 from ..views.asset_view import AssetManager
 from ..views.geometry_view import GeometryManager
 from ..core.navigation import Navigation
 # from ..views.geometry_view.geometry_file_manager import GeometryFileManager
 # from ..views.asset_view.asset_manager import AssetManager
 
 from ..app.project import content as project_content
 
 import shutil
 
 
+logger = getLogger('py_simultan_ui')
+
+
 project_dir = os.environ.get('PROJECT_DIR', '/simultan_projects')
 if not os.path.exists(project_dir):
     os.makedirs(project_dir)
 
 app.add_static_files('/project', project_dir)
 
 
@@ -360,92 +366,76 @@
     def download_project(self, e: events.ClickEventArguments):
         ui.download(f'project/{e.sender.project.project}')
 
 
 class ProjectManager(object):
     def __init__(self, *args, **kwargs):
 
-        self._data_model: Optional[DataModel, None] = None
-        self._view_manager: Optional[ViewManager, None] = None
-        self._asset_manager: Optional[AssetManager, None] = None
-        self._geometry_manager: Optional[GeometryManager, None] = None
-
+        self.user_manager: UserManager = kwargs.get('user_manager', user_manager)
         self._projects = None
         self.project_list = None
         self.mapped_data = None
-        self.mapper: Optional[PythonMapper, None] = kwargs.get('mapper', core.mapper)
 
-        self.view_manager = ViewManager(mapper=self.mapper, parent=self)
-        self.asset_manager = AssetManager(data_model=self.data_model)
-        self.geometry_manager = GeometryManager(mapper=self.mapper,
-                                                project_manager=self,
-                                                data_model=self.data_model)
-
-        self.navigation = Navigation(view_manager=self.view_manager,
-                                     asset_manager=self.asset_manager,
-                                     geometry_manager=self.geometry_manager,
-                                     )
-
-        self.detail_view = None
-
-        # self.geometry_file_manager = GeometryFileManager()
-        # self.asset_manager = AssetManager()
-        # FileInfo.__cls_type_view__ = self.asset_manager
-        # core.geometry_file_manager = self.geometry_file_manager
-        # core.asset_manager = self.asset_manager
+        if kwargs.get('data_model', None) is not None:
+            self.data_model = kwargs.get('data_model', None)
 
     @property
-    def data_model(self):
-        return self._data_model
+    def mapper(self) -> PythonMapper:
+        return self.user.mapper
 
-    @data_model.setter
-    def data_model(self, value):
-        self._data_model = value
-        core.data_model = value
+    @mapper.setter
+    def mapper(self, value: PythonMapper):
+        self.user.mapper = value
 
-        if self._data_model is not None:
-            app.add_static_files('/assets', self._data_model.project.ProjectUnpackFolder.FullPath)
+    @property
+    def view_manager(self) -> ViewManager:
+        return self.user.view_manager
 
-        for item in [self.view_manager, self.asset_manager, self.geometry_manager, self.navigation]:
-            if item is not None:
-                item.data_model = value
+    @property
+    def asset_manager(self) -> AssetManager:
+        return self.user.asset_manager
 
     @property
-    def view_manager(self) -> ViewManager:
-        return self._view_manager
+    def geometry_manager(self) -> GeometryManager:
+        return self.user.geometry_manager
 
-    @view_manager.setter
-    def view_manager(self, value: Optional[ViewManager]):
-        self._view_manager = value
-        core.view_manager = value
-
-    @property
-    def asset_manager(self):
-        return self._asset_manager
-
-    @asset_manager.setter
-    def asset_manager(self, value):
-        self._asset_manager = value
-        core.asset_manager = value
-
-    @property
-    def geometry_manager(self):
-        return self._geometry_manager
-
-    @geometry_manager.setter
-    def geometry_manager(self, value):
-        self._geometry_manager = value
-        core.geometry_manager = value
-        # orig_init = deepcopy(GeometryModel.__init__)
-        #
-        # def new_init(self, *args, **kwargs):
-        #     orig_init(self, *args, **kwargs)
-        #     # value.add_item_to_view(self)
-        #
-        # GeometryModel.__init__ = new_init
+    @property
+    def navigation(self) -> Navigation:
+        return self.user.navigation
+
+    @property
+    def detail_view(self):
+        return self.user.detail_view
+
+    @property
+    def home_tab(self):
+        return self.user.home_tab
+
+    @property
+    def project_tab(self):
+        return self.user.project_tab
+
+    @property
+    def user(self) -> User:
+        return self.user_manager.users[app.storage.user['username']]
+
+    @property
+    def data_model(self) -> Optional[DataModel]:
+        return self.user.data_model
+
+    @data_model.setter
+    def data_model(self, value: Optional[DataModel]):
+        logger.debug(f'Setting data model to {value}')
+        self.user.data_model = value
+        if self.user.data_model is not None:
+            app.add_static_files('/assets', self.user.data_model.project.ProjectUnpackFolder.FullPath)
+
+        for item in [self.view_manager, self.asset_manager, self.geometry_manager]:
+            if item is not None:
+                item.data_model = self.user.data_model
 
     @property
     def projects(self):
         # get list of files in project_dir
         self._projects = os.listdir(project_dir)
         return self._projects
 
@@ -458,75 +448,81 @@
                        *args,
                        **kwargs):
 
         shutil.copyfileobj(e.content, open(f'{project_dir}/{e.name}', 'wb'))
         ui.notify(f'Project {e.name} uploaded!')
         self.project_list.ui_content.refresh()
 
-    async def refresh_all_items(self, e):
-        await self.view_manager.refresh_all_items()
+    def refresh_all_items(self, e):
+        self.view_manager.refresh_all_items()
         self.asset_manager.update_items_views()
         self.geometry_manager.update_items_views()
         self.navigation.ui_content.refresh()
 
     def ui_content(self):
-        with core.project_tab:
+        with self.project_tab:
             self.view_manager.ui_content()
             self.asset_manager.ui_content()
             self.geometry_manager.ui_content()
             self.navigation.ui_content()
 
             with ui.page_sticky(position='bottom-right', x_offset=20, y_offset=20):
                 ui.button(on_click=self.refresh_all_items, icon='update').props('fab color=accent')
 
+        if self.data_model is None:
+            selected = None
+        else:
+            selected = os.path.basename(self.data_model.project.ProjectFile.FullPath)
+
         self.project_list = ProjectList(project_manager=self,
-                                        selected_project=app.storage.user.get('selected_project',
-                                                                              None)
+                                        selected_project=selected
                                         )
         self.project_list.ui_content()
 
         new_project_dialog = NewProjectDialog(parent=self)
         new_project_dialog.ui_content()
 
         ui.button('New project', on_click=new_project_dialog.dialog.open).classes('max-w-full')
 
         ui.upload(label='Upload simultan project',
                   on_upload=self.upload_project).on(
             'finish', lambda: ui.notify('Finish!')
         ).classes('max-w-full')
 
-    def open_project(self, e: events.ClickEventArguments):
+    def open_project(self, e: events.ClickEventArguments = None, *args, **kwargs):
+
+        if e is not None:
+            project = e.sender.project
+        else:
+            project = kwargs.get('project', None)
+
+        logger.info(f'Opening project {project.project}')
 
         n = ui.notification(timeout=None)
         n.spinner = True
-        n.message = f'Opening project {e.sender.project.project}'
+        n.message = f'Opening project {project.project}'
 
-        project_dict = e.sender.project.project_dict
+        project_dict = project.project_dict
         new_data_model = DataModel(project_path=project_dict['path'],
                                    user_name='admin',
                                    password='admin')
         self.mapped_data = new_data_model.get_typed_data(self.mapper, create_all=False)
         self.data_model = new_data_model
-        py_simultan_config.default_mapper = self.mapper
-        py_simultan_config.default_data_model = self.data_model
-        e.sender.project.selected = True
-        # self.project_list.ui_content.refresh()
-        n.message = 'Done!'
+        project.selected = True
+        self.project_list.ui_content.refresh()
+        n.message = f'Project {project.project} opened!'
         n.spinner = False
-        # self.method(*args, **kwargs)
         n.dismiss()
 
-        ui.notify(f'Project loaded with {len(self.mapped_data)} objects!')
-
     def close_project(self, e):
         if self.data_model is not None:
             self.data_model.cleanup()
         self.mapper.clear()
         self.mapped_data = []
         self.data_model = None
-        py_simultan_config.default_data_model = None
         ui.notify('Project closed!')
-        # self.project_list.ui_content.refresh()
+        self.project_list.ui_content.refresh()
         e.sender.project.selected = False
+        self.project_list.ui_content.refresh()
 
         # self.geometry_file_manager.geometry_models = []
         # project_content.refresh()
```

### Comparing `pysimultanui-0.1/src/core/tools.py` & `pysimultanui-0.2/src/core/tools.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.1/src/views/asset_view/asset_manager.py` & `pysimultanui-0.2/src/views/asset_view/asset_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 class AssetManager(TypeViewManager):
 
     item_view_name = 'Assets'
     item_view_cls = AssetView
     cls = FileInfo
 
     def __init__(self, *args, **kwargs):
-        self.mapper = kwargs.get('mapper', core.mapper)
-        self.project_manager = kwargs.get('project_manager', core.project_manager)
         super().__init__(*args, **kwargs)
 
     def update_items(self) -> list[any]:
         if self.data_model is None:
             return []
         assets = self.data_model.project_data_manager.AssetManager.Resources
         return [FileInfo(resource_entry=asset) for asset in assets]
```

### Comparing `pysimultanui-0.1/src/views/asset_view/asset_view.py` & `pysimultanui-0.2/src/views/asset_view/asset_view.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.1/src/views/component_dict_view/component_dict_manager.py` & `pysimultanui-0.2/src/views/component_dict_view/component_dict_manager.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.1/src/views/component_dict_view/component_dict_view.py` & `pysimultanui-0.2/src/views/component_dict_view/component_dict_view.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from nicegui import ui
 
 from ..type_view import TypeView
-from nicegui import ui
+from nicegui import ui, app
 
-from ... import core
+from ..detail_views import show_detail
+from ... import user_manager
 from ...core.edit_dialog import DictEditDialog
 from PySimultan2.simultan_object import SimultanObject
 from PySimultan2.default_types import ComponentDictionary
 
 from ..parameter_view import ParameterView
 from ..mapped_cls.mapped_cls_view import ContentItemView
 
@@ -31,15 +32,15 @@
 
             val = self.component
             if isinstance(val, SimultanObject):
                 if val.__ui_element__ is None:
                     self.view_manager.cls_views[val.__class__]['item_view_manager'].add_item_to_view(val)
                 with ui.item_section():
                     ui.label(f'{val.name}')
-                    ui.button('Details', on_click=val.__ui_element__.show_details)
+                    ui.button('Details', on_click=lambda e: show_detail(val))
                 with ui.item_section():
                     ui.label(f'{val.id}')
             elif isinstance(val, (int, float, str)):
                 with ui.item_section():
                     raw_val = self.parent.component.get_raw_attr(self.key)
                     ParameterView(component=val,
                                   raw_val=raw_val,
@@ -61,15 +62,15 @@
         raise NotImplementedError
 
     def remove(self, event):
         ui.notify('Edit not implemented yet', type='negative')
         raise NotImplementedError
 
 
-class ListContentView(object):
+class DictView(object):
 
     def __init__(self, *args, **kwargs):
         self.component: ComponentDictionary = kwargs.get('component')
         self.parent = kwargs.get('parent')
         self.card = None
 
         self.content_item_views: dict[str: ContentItemView] = {}
@@ -105,30 +106,67 @@
                           ).classes('w-full h-full').bind_text_from(self,
                                                                     'data',
                                                                     lambda x: f'Content ({len(self.component)})'
                                                                     ) as self.card:
             self.list_content()
 
 
+class DictDetailView(object):
+
+    def __init__(self, *args, **kwargs):
+        self.component: ComponentDictionary = kwargs.get('component')
+        self.parent = kwargs.get('parent')
+        self.card = None
+
+        self.content_view = DictView(component=self.component, parent=self)
+
+    def add_new_item(self, event):
+        self.parent.add_new_item(event)
+
+    def ui_content(self, *args, **kwargs):
+        with ui.row().classes('w-full h-full'):
+            ui.input(label='Name', value=self.component.name).bind_value(self.component, 'name')
+
+        with ui.row().classes('w-full h-full'):
+            ui.label('ID: ')
+            with ui.row():
+                with ui.row():
+                    ui.label(f'{self.component.Id.GlobalId.ToString()}')
+                with ui.row():
+                    ui.label(f'{self.component.Id.LocalId}')
+
+        content_view = DictView(component=self.component, parent=self)
+        content_view.ui_content()
+
+    def refresh(self):
+        self.ui_content()
+
+
 class ComponentDictView(TypeView):
 
+    detail_view = DictDetailView
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     @property
     def view_manager(self):
         return self.parent.view_manager
 
     @ui.refreshable
     def ui_content(self):
 
         with ui.card().classes(f"{self.colors['item']} w-full h-full") as self.card:
-            self.card.on('click', self.show_details)
+            self.card.on('click', show_detail(self.component,
+                                              parent=self.parent)
+                         )
             with ui.row().classes(f"{self.colors['item']} w-full") as self.row:
-                self.row.on('click', self.show_details)
+                self.row.on('click', show_detail(self.component,
+                                                 parent=self.parent)
+                            )
                 self.checkbox = ui.checkbox(on_change=self.select)
                 ui.input(label='Name', value=self.component.name).bind_value(self.component, 'name')
                 ui.label(f'{str(self.component.id)}')
 
     def add_new_item(self, event):
 
         parent = self
@@ -156,30 +194,9 @@
             parent.content_view.ui_content.refresh()
             edit_dialog.close()
 
         edit_dialog.save = save
         edit_dialog.create_edit_dialog()
 
     def show_details(self, *args, **kwargs):
-        TypeView.show_details(self)
-
-        core.detail_view.clear()
-        with core.detail_view as detail_view:
-            with ui.card().classes('w-full h-full'):
-                if kwargs.get('previous', None) is not None:
-                    with ui.row():
-                        ui.button(on_click=lambda e: kwargs.get('previous').__ui_element__.show_details(previous=self),
-                                  icon='arrow_back').classes('q-mr-md')
-
-                with ui.row().classes('w-full h-full'):
-                    ui.input(label='Name', value=self.component.name).bind_value(self.component, 'name')
-
-                with ui.row().classes('w-full h-full'):
-                    ui.label('ID: ')
-                    with ui.row():
-                        with ui.row():
-                            ui.label(f'{self.component.Id.GlobalId.ToString()}')
-                        with ui.row():
-                            ui.label(f'{self.component.Id.LocalId}')
-
-                content_view = ListContentView(component=self.component, parent=self)
-                content_view.ui_content()
+        self.detail_view(component=self.component,
+                         parent=self).ui_content()
```

### Comparing `pysimultanui-0.1/src/views/component_list_view/component_list_manager.py` & `pysimultanui-0.2/src/views/component_list_view/component_list_manager.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.1/src/views/component_list_view/component_list_view.py` & `pysimultanui-0.2/src/views/component_list_view/component_list_view.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from nicegui import ui
-
+import logging
 from ..type_view import TypeView
-from nicegui import ui
+from nicegui import ui, app
 
-from ... import core
+from ... import user_manager
+# from ... import core
+from ..detail_views import show_detail
 from ...core.edit_dialog import ContentEditDialog
 from PySimultan2.simultan_object import SimultanObject
 from PySimultan2.default_types import ComponentList
 
 from ..parameter_view import ParameterView
 from ..mapped_cls.mapped_cls_view import ContentItemView
 
+logger = logging.getLogger('py_simultan_ui')
+
 
 class ListItemView(object):
 
     def __init__(self, *args, **kwargs):
         self.component: SimultanObject = kwargs.get('component')
         self.parent = kwargs.get('parent')
         self.item_no = kwargs.get('item_no')
+        self.first = kwargs.get('first', False)
+        self.last = kwargs.get('last', False)
 
     @property
     def view_manager(self):
         return self.parent.view_manager
 
     @ui.refreshable
     def ui_content(self):
@@ -38,15 +44,15 @@
             #     ui.label(f'{self.component.name}').on('click', self.component.__ui_element__.show_details)
                 # ui.link(self.component.name, self.component.__ui_element__.card)
 
             with ui.item_section():
                 ui.label(f'{self.component.name}')
 
             with ui.item_section():
-                ui.button(on_click=lambda e: self.component.__ui_element__.show_details(previous=self.parent.component),
+                ui.button(on_click=lambda e: show_detail(self.component),
                           icon='launch').classes('q-ml-auto')
 
             with ui.item_section():
                 with ui.row():
                     ui.label(f'{self.component.Id.GlobalId.ToString()}')
                 with ui.row():
                     ui.label(f'{self.component.Id.LocalId}')
@@ -54,23 +60,29 @@
             with ui.item_section():
                 button = ui.button(on_click=self.edit,
                                    icon='edit').classes('q-ml-auto')
                 button.item = self.component
                 button.item_no = self.item_no
             with ui.item_section():
                 with ui.row():
-                    button = ui.button(on_click=self.move_up,
-                                       icon='keyboard_arrow_up').classes('q-ml-auto')
-                    button.item = self.component
-                    button.item_no = self.item_no
-                with ui.row():
-                    button = ui.button(on_click=self.move_down,
-                                       icon='keyboard_arrow_down').classes('q-ml-auto')
-                    button.item = self.component
-                    button.item_no = self.item_no
+                    if not self.first:
+                        button = ui.button(on_click=self.move_up,
+                                           icon='keyboard_arrow_up').classes('q-ml-auto')
+                        button.item = self.component
+                        button.item_no = self.item_no
+                    else:
+                        ui.label('')
+                with ui.row():
+                    if not self.last:
+                        button = ui.button(on_click=self.move_down,
+                                           icon='keyboard_arrow_down').classes('q-ml-auto')
+                        button.item = self.component
+                        button.item_no = self.item_no
+                    else:
+                        ui.label('')
 
             with ui.item_section():
                 button = ui.button(on_click=self.remove,
                                    icon='delete').classes('q-ml-auto')
                 button.item = self.component
                 button.item_no = self.item_no
 
@@ -88,15 +100,15 @@
 
     def move_down(self, event):
         if self.item_no < len(self.parent.component) - 1:
             self.parent.component.move_item(event.sender.item, event.sender.item_no + 1)
         self.parent.list_content.refresh()
 
 
-class ListContentView(object):
+class ListView(object):
 
     def __init__(self, *args, **kwargs):
         self.component: ComponentList = kwargs.get('component')
         self.parent = kwargs.get('parent')
         self.card = None
 
         self.content_item_views: dict[str: ContentItemView] = {}
@@ -110,77 +122,113 @@
         with ui.list().classes('w-full h-full'):
 
             for i, item in enumerate(self.component):
 
                 if self.content_item_views.get(i, None) is None or self.content_item_views[i].component != item:
                     self.content_item_views[i] = ListItemView(component=item,
                                                               parent=self,
-                                                              item_no=i)
+                                                              item_no=i,
+                                                              first=i == 0,
+                                                              last=i == len(self.component) - 1)
                 self.content_item_views[i].ui_content()
                 ui.separator()
 
-        ui.button(f'Add new item to {self.component.name}',
-                  on_click=self.parent.add_new_item, icon='add').classes('q-ml-auto')
+        try:
+            ui.button(f'Add new item to {self.component.name}',
+                      on_click=self.parent.add_new_item, icon='add').classes('q-ml-auto')
+        except Exception as e:
+            logger.error(f'Error adding new item: {e}')
 
     @ui.refreshable
     def ui_content(self):
         with ui.expansion(icon='format_list_bulleted',
                           text=f'Content ({len(self.component)})',
                           value=True
                           ).classes('w-full h-full').bind_text_from(self,
                                                                     'data',
                                                                     lambda x: f'Content ({len(self.component)})'
                                                                     ) as self.card:
             self.list_content()
 
 
+class ListDetailView(object):
+
+    def __init__(self, *args, **kwargs):
+        self.component: ComponentList = kwargs.get('component')
+        parent = kwargs.get('parent')
+
+    def ui_content(self, *args, **kwargs):
+
+        if kwargs.get('previous', None) is not None:
+            with ui.row():
+                ui.button(on_click=lambda e: show_detail(kwargs.get('previous')),
+                          icon='arrow_back').classes('q-mr-md')
+
+        with ui.item().classes('w-full h-full'):
+            with ui.item_section():
+                self.checkbox = ui.checkbox()
+            with ui.item_section():
+                ui.input(label='Name', value=self.component.name).bind_value(self.component, 'name')
+            with ui.item_section():
+                with ui.row():
+                    ui.label(f'{self.component.Id.GlobalId.ToString()}')
+                with ui.row():
+                    ui.label(f'{self.component.Id.LocalId}')
+        content_view = ListView(component=self.component, parent=self)
+        content_view.ui_content()
+
+    def add_new_item(self, event):
+
+        component = self.component
+        edit_dialog = ContentEditDialog(component=None,
+                                        parent=self,
+                                        content=None,
+                                        options=['Component'])
+
+        def save(self, *args, **kwargs):
+            if isinstance(edit_dialog.edit_dialog.value, list):
+                component.extend(edit_dialog.edit_dialog.value)
+            else:
+                component.append(edit_dialog.edit_dialog.value)
+            component.__ui_element__.content_view.list_content.refresh()
+            edit_dialog.close()
+
+        edit_dialog.save = save
+        edit_dialog.create_edit_dialog()
+
+    def refresh(self):
+        self.ui_content()
+
+
 class ComponentListView(TypeView):
 
+    detail_view = ListDetailView
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     @property
     def view_manager(self):
         return self.parent.view_manager
 
     @ui.refreshable
     def ui_content(self):
         with ui.card().classes(f"{self.colors['item']} w-full h-full") as self.card:
-            self.card.on('click', self.show_details)
+            self.card.on('click', show_detail(self.component))
             with ui.row().classes('bg-stone-100 w-full') as self.row:
-                self.row.on('click', self.show_details)
+                self.row.on('click', show_detail(self.component))
                 self.checkbox = ui.checkbox()
                 ui.input(label='Name', value=self.component.name).bind_value(self.component, 'name')
                 ui.label(f'{str(self.component.id)}')
 
             # self.content_view.ui_content()
 
     def show_details(self, *args, **kwargs):
-        TypeView.show_details(self)
-
-        core.detail_view.clear()
-        with core.detail_view as detail_view:
-            with ui.card().classes('w-full h-full').props('color="blue-800" keep-color') as self.card:
-                if kwargs.get('previous', None) is not None:
-                    with ui.row():
-                        ui.button(on_click=lambda e: kwargs.get('previous').__ui_element__.show_details(previous=self),
-                                  icon='arrow_back').classes('q-mr-md')
-
-                with ui.item().classes('w-full h-full'):
-                    with ui.item_section():
-                        self.checkbox = ui.checkbox()
-                    with ui.item_section():
-                        ui.input(label='Name', value=self.component.name).bind_value(self.component, 'name')
-                    with ui.item_section():
-                        with ui.row():
-                            ui.label(f'{self.component.Id.GlobalId.ToString()}')
-                        with ui.row():
-                            ui.label(f'{self.component.Id.LocalId}')
-                content_view = ListContentView(component=self.component, parent=self)
-                content_view.ui_content()
+        self.detail_view(component=self.component,
+                         parent=self).ui_content()
 
     def add_new_item(self, event):
 
         component = self.component
         edit_dialog = ContentEditDialog(component=None,
                                         parent=self,
                                         content=None,
```

### Comparing `pysimultanui-0.1/src/views/geometry_view/geometry_manager.py` & `pysimultanui-0.2/src/views/geometry_view/geometry_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import shutil
-
-from nicegui import ui, events
-from . import GeometryView
+from nicegui import ui, events, app
 from PySimultan2.geometry import GeometryModel
 
+from ... import user_manager
+from . import GeometryView
 from ..type_view_manager import TypeViewManager
-from ... import core
+from ... import user_manager
 
 
 try:
     import FreeCAD
     freecad_supported = True
 
     from ...core.freecad_utils.tools import import_freecad
@@ -21,20 +21,29 @@
 class GeometryManager(TypeViewManager):
 
     item_view_name = 'Geometry Models'
     item_view_cls = GeometryView
     cls = GeometryModel
 
     def __init__(self, *args, **kwargs):
-        self.mapper = kwargs.get('mapper', core.mapper)
-        self.project_manager = kwargs.get('project_manager', core.project_manager)
         super().__init__(*args, **kwargs)
-
         self.new_model_dialog = None
 
+    @property
+    def user(self):
+        return user_manager[app.storage.user['username']]
+
+    @property
+    def mapper(self):
+        return self.user.mapper
+
+    @property
+    def project_manager(self):
+        return self.user.project_manager
+
     def update_items(self) -> list[any]:
         if self.data_model is None:
             return []
 
         return [GeometryModel(wrapped_object=x,
                               object_mapper=self.mapper,
                               data_model=self.data_model) for x in
@@ -52,24 +61,14 @@
 
             self.expansion.bind_text_from(self,
                                           'items',
                                           lambda x: f'{self.item_view_name} ({len(x)})'
                                           )
 
             self.methods_ui_content()
-
-            # with ui.expansion(icon='format_list_bulleted', text='Methods').classes('w-full h-full'):
-            #     with ui.list().classes('w-full h-full'):
-            #         if freecad_supported:
-            #             with ui.item().classes('w-full h-full'):
-            #                 with ui.item_section().classes('w-full h-full'):
-            #                     ui.label('Import from file')
-            #                 with ui.item_section().classes('w-full h-full'):
-            #                     ui.button('Import', on_click=self.import_from_file).classes('q-ml-auto')
-
             self.items_ui_element = ui.row().classes('w-full h-full')
 
             if len(self.items) == 0:
                 with self.items_ui_element:
                     ui.label('No items to display')
             else:
                 for item in self.items:
@@ -79,15 +78,16 @@
                 self.button_create_ui_content()
 
         # super().ui_content()
 
     def create_new_model(self):
         def create_new_model_action():
             try:
-                new_model = GeometryModel(data_model=core.project_manager.data_model,
+
+                new_model = GeometryModel(data_model=self.user.data_model,
                                           name=self.new_model_dialog.project_name.value)
                 self._geometry_models = None
                 self._geometry_model_views = None
                 self.new_model_dialog.close()
                 ui.notify('New model created', type='positive')
                 self.add_item_to_view(new_model)
             except Exception as e:
@@ -134,15 +134,15 @@
             ui.notify(f'Project {e.name} uploaded!')
 
             # open file in FreeCAD
             doc = FreeCAD.open(local_path)
             num_created = import_freecad(doc=doc,
                                          geo_model=self.selected_items[0],
                                          data_model=self.data_model,
-                                         object_mapper=core.mapper,
+                                         object_mapper=self.user.mapper,
                                          scale=float(e.sender.scale_input.value))
 
             ui.notify(f'Imported {num_created[0]} Vertices, '
                       f'{num_created[1]} Edges, '
                       f'{num_created[2]} EdgeLoops, '
                       f'{num_created[3]} Faces, '
                       f'{num_created[4]} Volumes.', type='positive')
@@ -155,7 +155,9 @@
     def methods_ui_content(self):
         with ui.expansion(icon='code', text='Methods').classes('w-full h-full bg-stone-300'):
             with ui.list().classes('w-full h-full'):
                 if freecad_supported:
                     with ui.row().classes('w-full h-full'):
                         ui.label('Import from file')
                         ui.button('Import', on_click=self.import_from_file).classes('q-ml-auto')
+                else:
+                    ui.label('No Methods registered (FreeCAD not supported)')
```

### Comparing `pysimultanui-0.1/src/views/geometry_view/geometry_view.py` & `pysimultanui-0.2/src/views/geometry_view/geometry_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,119 +1,99 @@
 import os
-from nicegui import ui, events, app
-from .tools import create_stl_file
-from ..type_view import TypeView
 
 from PySimultan2.geometry import GeometryModel
+from nicegui import ui, events, app
 
-from ... import core
+# from ..detail_views import show_detail
+from .tools import create_stl_file
+from ..type_view import TypeView
+from ... import user_manager
 
 if not os.path.exists('/static/stl'):
     os.makedirs('/static/stl')
 
 app.add_static_files('/stl', '/static/stl')
 
 
-class GeometryView(TypeView):
+class GeometryDetailView(object):
 
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        self.component: GeometryModel = kwargs.get('component')
+        self.parent: GeometryView = kwargs.get('parent')
 
     @property
     def geometry_model(self) -> GeometryModel:
         return self.component
 
-    @ui.refreshable
-    def ui_content(self):
-
-        with ui.card().classes(f"{self.colors['item']} w-full h-full") as self.card:
-            self.card.on('click', self.show_details)
-            with ui.row().classes('bg-stone-100 w-full') as self.row:
-                self.row.on('click', self.show_details)
-                self.checkbox = ui.checkbox(on_change=self.select)
-                ui.label('Name:')
-                ui.label(self.geometry_model.name)
-                ui.label('Key:')
-                ui.label(self.geometry_model.key)
+    def ui_content(self, *args, **kwargs):
+        with ui.row():
+            ui.input(label='Name', value=self.component.name).bind_value(self.component, 'name')
+
+        with ui.row():
+            ui.label('Key:')
+            ui.label(self.geometry_model.key)
+
+        show_geo_button = ui.button('Show Geometry', on_click=self.show_geometry)
+
+        with ui.expansion(icon='format_list_bulleted',
+                          text=f'Geometry ({len(self.geometry_model.vertices)})').classes(
+            'w-full h-full'):
+
+            with ui.expansion(icon='format_list_bulleted',
+                              text=f'Vertices ({len(self.geometry_model.vertices)})').classes(
+                'w-full h-full') as exp:
+                with ui.list().classes('w-full h-full'):
+                    for vertex in self.geometry_model.vertices:
+                        with ui.item():
+                            with ui.item_section():
+                                ui.label(f'Vertex {vertex.id}')
+                            with ui.item_section():
+                                ui.label(f'x: {vertex.x}')
+                            with ui.item_section():
+                                ui.label(f'y: {vertex.y}')
+                            with ui.item_section():
+                                ui.label(f'z: {vertex.z}')
+
+            with ui.expansion(icon='format_list_bulleted',
+                              text=f'Edges ({len(self.geometry_model.edges)})').classes(
+                'w-full h-full') as exp:
+                with ui.list().classes('w-full h-full'):
+                    for edge in self.geometry_model.edges:
+                        with ui.item():
+                            with ui.item_section():
+                                ui.label(f'Edge {edge.id}')
+                            with ui.item_section():
+                                ui.label(f'Vertex 1: {edge.vertex_0.id}')
+                            with ui.item_section():
+                                ui.label(f'Vertex 2: {edge.vertex_1.id}')
+                            with ui.item_section():
+                                ui.label(f'Length: {edge.length}')
+
+            with ui.expansion(icon='format_list_bulleted',
+                              text=f'Faces ({len(self.geometry_model.faces)})').classes('w-full h-full') as exp:
+                with ui.list().classes('w-full h-full'):
+                    for face in self.geometry_model.faces:
+                        with ui.item():
+                            with ui.item_section():
+                                ui.label(f'Face {face.id}')
+                            with ui.item_section():
+                                ui.label(f'Area: {face.area}')
+
+            with ui.expansion(icon='format_list_bulleted',
+                              text=f'Volumes ({len(self.geometry_model.volumes)})').classes(
+                'w-full h-full') as exp:
+                with ui.list().classes('w-full h-full'):
+                    for volume in self.geometry_model.volumes:
+                        with ui.item():
+                            with ui.item_section():
+                                ui.label(f'Volume {volume.id}')
+                            with ui.item_section():
+                                ui.label(f'Volume: {volume.volume}')
 
-    def show_details(self, *args, **kwargs):
-        TypeView.show_details(self)
-
-        core.detail_view.clear()
-        with core.detail_view as detail_view:
-            with ui.card().classes('w-full h-full'):
-                if kwargs.get('previous', None) is not None:
-                    with ui.row():
-                        ui.button(on_click=lambda e: kwargs.get('previous').__ui_element__.show_details(previous=self),
-                                  icon='arrow_back').classes('q-mr-md')
-
-                with ui.row():
-                    ui.input(label='Name', value=self.component.name).bind_value(self.component, 'name')
-
-                with ui.row():
-                    ui.label('Key:')
-                    ui.label(self.geometry_model.key)
-
-                show_geo_button = ui.button('Show Geometry', on_click=self.show_geometry)
-
-                with ui.expansion(icon='format_list_bulleted',
-                                  text=f'Geometry ({len(self.geometry_model.vertices)})').classes(
-                    'w-full h-full'):
-
-                    with ui.expansion(icon='format_list_bulleted',
-                                      text=f'Vertices ({len(self.geometry_model.vertices)})').classes(
-                        'w-full h-full') as exp:
-                        with ui.list().classes('w-full h-full'):
-                            for vertex in self.geometry_model.vertices:
-                                with ui.item():
-                                    with ui.item_section():
-                                        ui.label(f'Vertex {vertex.id}')
-                                    with ui.item_section():
-                                        ui.label(f'x: {vertex.x}')
-                                    with ui.item_section():
-                                        ui.label(f'y: {vertex.y}')
-                                    with ui.item_section():
-                                        ui.label(f'z: {vertex.z}')
-
-                    with ui.expansion(icon='format_list_bulleted',
-                                      text=f'Edges ({len(self.geometry_model.edges)})').classes(
-                        'w-full h-full') as exp:
-                        with ui.list().classes('w-full h-full'):
-                            for edge in self.geometry_model.edges:
-                                with ui.item():
-                                    with ui.item_section():
-                                        ui.label(f'Edge {edge.id}')
-                                    with ui.item_section():
-                                        ui.label(f'Vertex 1: {edge.vertex_0.id}')
-                                    with ui.item_section():
-                                        ui.label(f'Vertex 2: {edge.vertex_1.id}')
-                                    with ui.item_section():
-                                        ui.label(f'Length: {edge.length}')
-
-                    with ui.expansion(icon='format_list_bulleted',
-                                      text=f'Faces ({len(self.geometry_model.faces)})').classes('w-full h-full') as exp:
-                        with ui.list().classes('w-full h-full'):
-                            for face in self.geometry_model.faces:
-                                with ui.item():
-                                    with ui.item_section():
-                                        ui.label(f'Face {face.id}')
-                                    with ui.item_section():
-                                        ui.label(f'Area: {face.area}')
-
-                    with ui.expansion(icon='format_list_bulleted',
-                                      text=f'Volumes ({len(self.geometry_model.volumes)})').classes('w-full h-full') as exp:
-                        with ui.list().classes('w-full h-full'):
-                            for volume in self.geometry_model.volumes:
-                                with ui.item():
-                                    with ui.item_section():
-                                        ui.label(f'Volume {volume.id}')
-                                    with ui.item_section():
-                                        ui.label(f'Volume: {volume.volume}')
-
-                delete_button = ui.button('Delete', on_click=self.delete_model)
+        delete_button = ui.button('Delete', on_click=self.delete_model)
 
     def delete_model(self, *args, **kwargs):
         ui.notify('Delete not implemented yet', type='negative')
 
     def show_geometry(self):
         # create dialog with geometry
         with ui.dialog() as dialog, ui.card().classes('w-full h-full'):
@@ -127,7 +107,42 @@
 
         dialog.open()
 
     def handle_click(self, e: events.SceneClickEventArguments, *args, **kwargs):
         hit = e.hits[0]
         name = hit.object_name or hit.object_id
         ui.notify(f'You clicked on the {name} at ({hit.x:.2f}, {hit.y:.2f}, {hit.z:.2f})')
+
+    def refresh(self):
+        self.ui_content()
+
+
+class GeometryView(TypeView):
+
+    detail_view = GeometryDetailView
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    @property
+    def geometry_model(self) -> GeometryModel:
+        return self.component
+
+    @ui.refreshable
+    def ui_content(self):
+        from ..detail_views import show_detail
+        with ui.card().classes(f"{self.colors['item']} w-full h-full") as self.card:
+            self.card.on('click', lambda e: show_detail(value=self.component,
+                                                        parent=self)
+                         )
+            with ui.row().classes('h-full w-full') as self.row:
+                self.row.on('click', lambda e: show_detail(value=self.component,
+                                                           parent=self)
+                            )
+                self.checkbox = ui.checkbox(on_change=self.select)
+                ui.label('Name:')
+                ui.label(self.geometry_model.name)
+                ui.label('Key:')
+                ui.label(self.geometry_model.key)
+
+    def delete_model(self, *args, **kwargs):
+        ui.notify('Delete not implemented yet', type='negative')
```

### Comparing `pysimultanui-0.1/src/views/geometry_view/tools.py` & `pysimultanui-0.2/src/views/geometry_view/tools.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.1/src/views/mapped_cls/mapped_cls_manager.py` & `pysimultanui-0.2/src/views/mapped_cls/mapped_cls_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from nicegui import ui
 from ..type_view_manager import TypeViewManager
 from PySimultan2.simultan_object import SimultanObject
-from ... import core
 
 
 class MappedClsManager(TypeViewManager):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -50,19 +49,19 @@
 
         with ui.row().classes('w-full h-full'):
             self.button_create_ui_content()
 
     @ui.refreshable
     def methods_content(self):
 
-        cls = core.mapper.mapped_classes.get(self.cls._taxonomy)
-        if cls not in core.method_mapper.mapped_methods.keys():
-            core.method_mapper.resolve_classes()
+        cls = self.user.mapper.mapped_classes.get(self.cls._taxonomy)
+        if cls not in self.user.method_mapper.mapped_methods.keys():
+            self.user.method_mapper.resolve_classes()
 
-        mapped_methods = core.method_mapper.mapped_methods.get(cls, [])
+        mapped_methods = self.user.method_mapper.mapped_methods.get(cls, [])
 
         with ui.expansion(icon='code', text='Methods').classes('w-full h-full bg-stone-200'):
             with ui.list().classes('w-full h-full'):
                 for method in mapped_methods:
                     with ui.item():
                         with ui.item_section():
                             ui.label(method.name)
```

### Comparing `pysimultanui-0.1/src/views/mapped_cls/mapped_cls_view.py` & `pysimultanui-0.2/src/views/mapped_cls/mapped_cls_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from nicegui import ui
 from numpy import ndarray
 from pandas import DataFrame
 
 from ..type_view import TypeView
-from nicegui import ui, events
+from ..type_view_manager import TypeViewManager
+from nicegui import ui, events, app
 
+from ... import user_manager
 from ... import core
 from ...core.edit_dialog import ContentEditDialog
 from PySimultan2.simultan_object import SimultanObject
 
+from ..detail_views import show_detail
 from ..parameter_view import ParameterView
 
 
 class ContentItemView(object):
     def __init__(self, *args, **kwargs):
         self.component: SimultanObject = kwargs.get('component')
         self.parent = kwargs.get('parent')
@@ -33,15 +36,16 @@
                 ui_simultan_object_ref(val, self)
             elif isinstance(val, (int, float, str)):
                 with ui.item_section():
                     raw_val = self.component.get_raw_attr(self.content.property_name)
                     ParameterView(component=val,
                                   raw_val=raw_val,
                                   content=self.content,
-                                  parent=self.parent, taxonomy=self.content).ui_content()
+                                  parent=self.parent,
+                                  taxonomy=self.content).ui_content()
 
             elif isinstance(val, (ndarray, DataFrame)):
                 ui_ndarray_ref(val, self)
             else:
                 if val is None:
                     with ui.item_section():
                         ui.label('None')
@@ -66,20 +70,23 @@
                                         parent=self.parent,
                                         content=event.sender.content)
         edit_dialog.create_edit_dialog()
 
 
 def ui_simultan_object_ref(val: SimultanObject,
                            parent: ContentItemView):
-    if val.__ui_element__ is None:
-        cls_view = parent.view_manager.cls_views.get(val.__class__, None)[
-            'item_view_manager'] if parent.view_manager.cls_views.get(val.__class__,
-                                                                    None) is not None else None
+
+    if not hasattr(val, '__ui_element__') or val.__ui_element__ is None:
+
+        view_manager = user_manager[app.storage.user['username']].project_manager.view_manager
+        cls_view = view_manager.cls_views.get(val.__class__, None)[
+            'item_view_manager'] if view_manager.cls_views.get(val.__class__,
+                                                               None) is not None else None
         if cls_view is None:
-            cls_view = parent.view_manager.create_mapped_cls_view_manager(taxonomy=val.__class__._taxonomy)[
+            cls_view: TypeViewManager = view_manager.create_mapped_cls_view_manager(taxonomy=val.__class__._taxonomy)[
                 'item_view_manager']
             if cls_view is None:
                 ui.label(f'No View for this class: {val.__class__}')
                 return
         try:
             cls_view.add_item_to_view(val)
         except KeyError:
@@ -89,15 +96,17 @@
         ui.label(f'No View for this object: {str(val), val.__class__}')
         return
 
     with ui.item_section():
         if val.__ui_element__ is not None:
             ui.label(val.name)
     with ui.item_section():
-        ui.button(on_click=lambda e: val.__ui_element__.show_details(previous=parent.component),
+        ui.button(on_click=lambda e: show_detail(value=val,
+                                                 parent=parent,
+                                                 previous=parent.component),
                   icon='launch').classes('q-ml-auto')
     with ui.item_section():
         with ui.row():
             ui.label(f'{val.id.GlobalId.ToString()}')
         with ui.row():
             ui.label(f'{val.id.LocalId}')
     with ui.item_section():
@@ -105,30 +114,31 @@
         edit_btn.item = val
         edit_btn.content = parent.content
 
 
 def ui_ndarray_ref(val: (ndarray, DataFrame),
                    parent: ContentItemView):
     raw_val = parent.component.get_raw_attr(parent.content.property_name)
+    view_manager = user_manager[app.storage.user['username']].project_manager.view_manager
 
     def get_ui_element():
-        ui_element = parent.view_manager.cls_views[val.__class__]['item_view_manager'].item_views.get(
+        ui_element = view_manager.cls_views[val.__class__]['item_view_manager'].item_views.get(
             str(raw_val.ValueSource.ValueField.Id), None)
         return ui_element
 
     ui_element = get_ui_element()
 
     if ui_element is None:
-        parent.view_manager.cls_views[val.__class__]['item_view_manager'].add_item_to_view(val, raw_val)
+        view_manager.cls_views[val.__class__]['item_view_manager'].add_item_to_view(val, raw_val)
     ui_element = get_ui_element()
 
     with ui.item_section():
         ui.label(raw_val.ValueSource.ValueField.Name)
-    with ui.item_section():
-        ui.button(on_click=lambda e: ui_element.show_details(previous=parent.component),
+        ui.button(on_click=lambda e: show_detail(value=val,
+                                                 parent=parent),
                   icon='launch').classes('q-ml-auto')
     with ui.item_section():
         ui.label(f'{raw_val.ValueSource.ValueField.Id}')
     with ui.item_section():
         edit_btn = ui.button(on_click=parent.edit, icon='edit').classes('q-ml-auto')
         edit_btn.item = val
         edit_btn.content = parent.content
@@ -147,30 +157,67 @@
     @property
     def view_manager(self):
         return self.parent.view_manager
 
     @ui.refreshable
     def ui_content(self):
         with ui.expansion(icon='format_list_bulleted', text='Content', value=True).classes('w-full h-full') as exp:
-            with ui.list().classes('w-full h-full'):
+            with ui.list().classes('w-full h-full').props('bordered separator'):
                 for content in self.component._taxonomy_map.content:
                     if self.content_item_views.get(content.property_name) is None:
                         self.content_item_views[content.property_name] = ContentItemView(component=self.component,
                                                                                          parent=self.parent,
                                                                                          content=content)
                     self.content_item_views[content.property_name].ui_content()
                     ui.separator()
 
 
+class MappedClsDetailView(object):
+
+    def __init__(self, *args, **kwargs):
+        self.component: SimultanObject = kwargs.get('component')
+        self.parent = kwargs.get('parent')
+        self.card = None
+        self.row = None
+
+        self.content_view = ContentView(component=self.component, parent=self.parent)
+
+    @property
+    def view_manager(self):
+        return self.parent.view_manager
+
+    @ui.refreshable
+    def ui_content(self, *args, **kwargs):
+
+        with ui.card().classes('w-full h-full'):
+            with ui.item().classes('w-full h-full'):
+                with ui.item_section():
+                    ui.input(label='Name', value=self.component.name).bind_value(self.component, 'name')
+                with ui.item_section():
+                    with ui.row():
+                        ui.label('Global ID: ')
+                        ui.label(f'{self.component.id.GlobalId.ToString()}')
+                    with ui.row():
+                        ui.label('Local ID: ')
+                        ui.label(f'{self.component.id.LocalId}')
+            content_view = ContentView(component=self.component, parent=self)
+            content_view.ui_content()
+
+    def refresh(self):
+        self.ui_content.refresh()
+
+
 class MappedClsView(TypeView):
 
     colors = {'item': 'bg-stone-100',
               'cls_color': 'bg-stone-300',
               'selected': 'bg-blue-200'}
 
+    detail_view = MappedClsDetailView
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     @property
     def view_manager(self):
         return self.parent.view_manager
 
@@ -182,39 +229,31 @@
         #             self.checkbox = ui.checkbox().classes('q-ml-auto')
         #         with ui.item_section().classes('w-full h-full'):
         #             ui.input(label='Name', value=self.component.name).bind_value(self.component, 'name')
         #         with ui.item_section().classes('w-full h-full'):
         #             ui.label(f'{str(self.component.id)}')
 
         with ui.card().classes(f"{self.colors['item']} w-full h-full") as self.card:
-            self.card.on('click', self.show_details)
+            self.card.on('click', lambda e: show_detail(value=self.component,
+                                                        parent=self)
+                         )
             with ui.row().classes(f"{self.colors['item']} w-full") as self.row:
-                self.row.on('click', self.show_details)
+                self.row.on('click', lambda e: show_detail(value=self.component,
+                                                           parent=self.component)
+                            )
                 self.checkbox = ui.checkbox(on_change=self.select)
                 ui.input(label='Name', value=self.component.name).bind_value(self.component, 'name')
                 with ui.row():
                     with ui.row():
+                        ui.label('Global ID: ')
                         ui.label(f'{self.component.id.GlobalId.ToString()}')
                     with ui.row():
+                        ui.label('Local ID: ')
                         ui.label(f'{self.component.id.LocalId}')
 
                 # with ui.item_section():
                 #     ui.button(on_click=self.show_details, icon='launch').classes('q-ml-auto')
             # self.content_view.ui_content()
 
     def show_details(self, *args, **kwargs):
-        TypeView.show_details(self)
-        core.detail_view.clear()
-        with core.detail_view as detail_view:
-            if kwargs.get('previous', None) is not None:
-                with ui.row():
-                    ui.button(on_click=lambda e: kwargs.get('previous').__ui_element__.show_details(previous=self),
-                              icon='arrow_back').classes('q-mr-md')
-
-            with ui.card().classes('w-full h-full'):
-                with ui.item().classes('w-full h-full'):
-                    with ui.item_section():
-                        ui.input(label='Name', value=self.component.name).bind_value(self.component, 'name')
-                    with ui.item_section():
-                        ui.label(f'{str(self.component.id)}')
-                content_view = ContentView(component=self.component, parent=self)
-                content_view.ui_content()
+        self.detail_view(component=self.component,
+                         parent=self).ui_content()
```

### Comparing `pysimultanui-0.1/src/views/numpy_view.py` & `pysimultanui-0.2/src/views/pandas_df_view.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,141 +1,159 @@
-import numpy as np
 import pandas as pd
 from typing import Type
 from nicegui import Client, app, ui, events
 from .type_view import TypeView
 from .type_view_manager import TypeViewManager
 
-from .. import core
-from ..core.edit_dialog import ContentEditDialog
+# from .. import user_manager
+# from .detail_views import show_detail
+# from ..core.edit_dialog import ContentEditDialog
 
 from SIMULTAN.Data.MultiValues import (SimMultiValueField3D, SimMultiValueField3DParameterSource, SimMultiValueBigTable,
                                        SimMultiValueBigTableHeader, SimMultiValueBigTableParameterSource)
 
-from PySimultan2.multi_values import simultan_multi_value_field_3d_to_numpy
+from PySimultan2.multi_values import simultan_multi_value_big_table_to_pandas
 
 
-class NDArrayView(TypeView):
+class DataFrameDetailView(object):
 
     def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-        self.content = kwargs.get('content', None)
+        self.component: SimMultiValueBigTable = kwargs.get('component')
+        self.parent = kwargs.get('parent')
         self.array = None
         self.dim_slider = None
         self.table = None
 
-    @ui.refreshable
-    def table_ui_content(self):
+    def ui_content(self, *args, **kwargs):
+
+        with ui.row().classes('w-full h-full'):
+            ui.input(label='Name',
+                     value=self.component.Name).classes('w-full h-full').bind_value(self.component,
+                                                                                    'Name')
+        with ui.row().classes('w-full h-full'):
+            with ui.column():
+                ui.label('ID:')
+                ui.label(f'{str(self.component.Id.GlobalId.ToString())}')
+                ui.label(f'{str(self.component.Id.LocalId)}')
+
+        df = simultan_multi_value_big_table_to_pandas(self.component)
+
+        with ui.row().classes('w-full h-full'):
+            with ui.column():
+                ui.label('Shape:')
+                ui.label(f'{df.shape}')
 
-        if self.array.shape.__len__() > 2:
-            disp_array = self.array[int(self.dim_slider.value if self.dim_slider is not None else 0), :, :]
-        else:
-            disp_array = self.array
-
-        self.table = ui.table.from_pandas(pd.DataFrame(disp_array)
-                                          ).classes('w-full h-full')
-        with self.table.add_slot('top-left'):
+        ui.separator()
+
+        table = ui.table.from_pandas(df).classes('w-full h-full')
+
+        with table.add_slot('top-left'):
             def toggle() -> None:
-                self.table.toggle_fullscreen()
-                button.props('icon=fullscreen_exit' if self.table.is_fullscreen else 'icon=fullscreen')
+                table.toggle_fullscreen()
+                button.props('icon=fullscreen_exit' if table.is_fullscreen else 'icon=fullscreen')
 
             button = ui.button('Toggle fullscreen', icon='fullscreen', on_click=toggle).props('flat')
 
+
+class DataFrameView(TypeView):
+
+    detail_view = DataFrameDetailView
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+    @property
+    def component(self):
+        return self._component
+
+    @component.setter
+    def component(self, value):
+        self._component = value
+
     @ui.refreshable
     def ui_content(self):
+        from .detail_views import show_detail
 
         with ui.card().classes(f"{self.colors['item']} w-full h-full") as self.card:
-            self.card.on('click', self.show_details)
+            self.card.on('click', lambda e: show_detail(value=self.component,
+                                                        parent=self))
             with ui.row().classes('bg-stone-100 w-full') as self.row:
-                self.row.on('click', self.show_details)
+                self.row.on('click', lambda e: show_detail(value=self.component,
+                                                           parent=self))
                 self.checkbox = ui.checkbox(on_change=self.select)
-                ui.label(f'{self.component.Id}')
-                ui.label(f'{self.component.Name}')
-
-        # with ui.card().classes('w-full h-full').props('color="blue-800" keep-color') as self.card:
-        #     with ui.list().classes('w-full h-full'):
-        #         with ui.item():
-        #             with ui.item_section().classes('max-w-40'):
-        #                 self.checkbox = ui.checkbox()
-        #             with ui.item_section():
-        #                 with ui.item():
-        #                     with ui.item_section():
-        #                         ui.label(f'ID:').props('font-weight=bold')
-        #                     with ui.item_section():
-        #                         ui.label(f'{self.component.Id}')
-        #                 with ui.item():
-        #                     with ui.item_section():
-        #                         ui.label(f'Name:').props('font-weight=bold')
-        #                     with ui.item_section():
-        #                         ui.label(f'{self.component.Name}')
-
-    def show_details(self, *args, **kwargs):
-        TypeView.show_details(self)
-
-        core.detail_view.clear()
-        with core.detail_view as detail_view:
-            with ui.card().classes('w-full h-full'):
-                if kwargs.get('previous', None) is not None:
-                    with ui.row():
-                        ui.button(on_click=lambda e: kwargs.get('previous').__ui_element__.show_details(previous=self),
-                                  icon='arrow_back').classes('q-mr-md')
-
                 with ui.row():
-                    ui.input(label='Name',
-                             value=self.component.Name).classes('w-full h-full').bind_value(self.component,
-                                                                                            'Name')
-                with ui.row():
-                    ui.label('ID:')
+                    ui.label('Name:').props('font-weight=bold')
+                    ui.input(value=self.component.Name).bind_value(self.component, 'Name')
+                    ui.label('ID:').props('font-weight=bold')
                     with ui.row():
                         with ui.row():
                             ui.label(f'{self.component.Id.GlobalId.ToString()}')
                         with ui.row():
                             ui.label(f'{self.component.Id.LocalId}')
 
-                ui.separator()
+    def show_details(self, *args, **kwargs):
 
-                self.array = simultan_multi_value_field_3d_to_numpy(self.component)
-                self.table_ui_content()
+        self.detail_view(component=self.component,
+                         parent=self).ui_content()
 
-                with ui.card().classes('w-full h-full'):
-                    ui.label('Select dimension to display:')
-                    self.dim_slider = ui.slider(min=0, max=self.array.shape[0] - 1,
-                                                step=1,
-                                                value=0,
-                                                on_change=self.table_ui_content.refresh)
-                    ui.input('dim_slider',
-                             value='0').bind_value(self.dim_slider,
-                                                   'value',
-                                                   forward=lambda x: int(x),
-                                                   backward=lambda x: str(x))
-
-
-class NDArrayManager(TypeViewManager):
-
-    cls: np.ndarray = np.ndarray
-    item_view_cls: Type[TypeView] = NDArrayView
-    item_view_name = 'ND Arrays'
+        # TypeView.show_details(self)
+        # core.detail_view.clear()
+        # with core.detail_view as detail_view:
+        #     with ui.card().classes('w-full h-full'):
+        #
+        #         if kwargs.get('previous', None) is not None:
+        #             with ui.row():
+        #                 ui.button(on_click=lambda e: kwargs.get('previous').__ui_element__.show_details(previous=self),
+        #                           icon='arrow_back').classes('q-mr-md')
+        #
+        #         with ui.row():
+        #             ui.input(label='Name',
+        #                      value=self.component.Name).classes('w-full h-full').bind_value(self.component,
+        #                                                                                     'Name')
+        #         with ui.row():
+        #             ui.label('ID:')
+        #             ui.label(f'{str(self.component.Id)}')
+        #
+        #         ui.separator()
+        #
+        #         table = ui.table.from_pandas(simultan_multi_value_big_table_to_pandas(self.component)
+        #                                      ).classes('w-full h-full')
+        #
+        #         with table.add_slot('top-left'):
+        #             def toggle() -> None:
+        #                 table.toggle_fullscreen()
+        #                 button.props('icon=fullscreen_exit' if table.is_fullscreen else 'icon=fullscreen')
+        #
+        #             button = ui.button('Toggle fullscreen', icon='fullscreen', on_click=toggle).props('flat')
+
+
+class DataFrameManager(TypeViewManager):
+
+    cls: pd.DataFrame = pd.DataFrame
+    item_view_cls: Type[TypeView] = DataFrameView
+    item_view_name = 'Dataframes'
 
-    def update_items(self) -> list[SimMultiValueField3D]:
+    def button_create_ui_content(self):
+        ui.button('Create new DataFrame', on_click=self.create_new_item, icon='add')
+
+    def update_items(self) -> list[SimMultiValueBigTable]:
         if self.data_model is None:
             return []
-        return [x for x in self.data_model.value_fields if type(x) == SimMultiValueField3D]
 
-    def button_create_ui_content(self):
-        ui.button('Create new ND-Array', on_click=self.create_new_item, icon='add')
+        return [x for x in self.data_model.value_fields if type(x) == SimMultiValueBigTable]
 
     @ui.refreshable
     def add_item_to_view(self,
                          item: any,
                          raw_val=None):
 
-        if isinstance(item, SimMultiValueField3D):
+        if isinstance(item, SimMultiValueBigTable):
             val_source = item
-        elif isinstance(item, np.ndarray):
-            val_source: SimMultiValueField3D = raw_val.ValueSource.ValueField
+        elif isinstance(item, pd.DataFrame):
+            val_source: SimMultiValueBigTable = raw_val.ValueSource.ValueField
 
         if self.items_ui_element is None:
             return
 
         if val_source not in self.items:
             self.items.append(val_source)
         item_view = self.item_views.get(str(val_source.Id), None)
```

### Comparing `pysimultanui-0.1/src/views/pandas_df_view.py` & `pysimultanui-0.2/src/views/numpy_view.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,143 @@
+import numpy as np
 import pandas as pd
 from typing import Type
 from nicegui import Client, app, ui, events
 from .type_view import TypeView
 from .type_view_manager import TypeViewManager
 
-from .. import core
+# from .detail_views import show_detail
+from .. import user_manager
 from ..core.edit_dialog import ContentEditDialog
 
 from SIMULTAN.Data.MultiValues import (SimMultiValueField3D, SimMultiValueField3DParameterSource, SimMultiValueBigTable,
                                        SimMultiValueBigTableHeader, SimMultiValueBigTableParameterSource)
 
-from PySimultan2.multi_values import simultan_multi_value_big_table_to_pandas
+from PySimultan2.multi_values import simultan_multi_value_field_3d_to_numpy
 
 
-class DataFrameView(TypeView):
+class NDArrayDetailView(object):
 
     def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-
-    @property
-    def component(self):
-        return self._component
-
-    @component.setter
-    def component(self, value):
-        self._component = value
-
-    @ui.refreshable
-    def ui_content(self):
-        with ui.card().classes(f"{self.colors['item']} w-full h-full") as self.card:
-            self.card.on('click', self.show_details)
-            with ui.row().classes('bg-stone-100 w-full') as self.row:
-                self.row.on('click', self.show_details)
-                self.checkbox = ui.checkbox(on_change=self.select)
-                with ui.row():
-                    ui.label('Name:').props('font-weight=bold')
-                    ui.input(value=self.component.Name).bind_value(self.component, 'Name')
-                    ui.label('ID:').props('font-weight=bold')
-                    with ui.row():
-                        with ui.row():
-                            ui.label(f'{self.component.Id.GlobalId.ToString()}')
-                        with ui.row():
-                            ui.label(f'{self.component.Id.LocalId}')
+        self.component: SimMultiValueField3D = kwargs.get('component')
+        self.parent = kwargs.get('parent')
+        self.array = None
+        self.dim_slider = None
+        self.table = None
+
+    def ui_content(self, *args, **kwargs):
+        from .detail_views import show_detail
+        detail_view = user_manager[app.storage.user['username']].detail_view
 
-    def show_details(self, *args, **kwargs):
-        TypeView.show_details(self)
-        core.detail_view.clear()
-        with core.detail_view as detail_view:
+        detail_view.clear()
+        with detail_view:
             with ui.card().classes('w-full h-full'):
-
                 if kwargs.get('previous', None) is not None:
                     with ui.row():
-                        ui.button(on_click=lambda e: kwargs.get('previous').__ui_element__.show_details(previous=self),
+                        ui.button(on_click=lambda e: show_detail(kwargs.get('previous')),
                                   icon='arrow_back').classes('q-mr-md')
 
                 with ui.row():
                     ui.input(label='Name',
                              value=self.component.Name).classes('w-full h-full').bind_value(self.component,
                                                                                             'Name')
-                with ui.row():
+                with ui.row().classes('w-full h-full'):
                     ui.label('ID:')
-                    ui.label(f'{str(self.component.Id)}')
+                    with ui.row():
+                        with ui.row():
+                            ui.label(f'{self.component.Id.GlobalId.ToString()}')
+                        with ui.row():
+                            ui.label(f'{self.component.Id.LocalId}')
+
+                self.array = simultan_multi_value_field_3d_to_numpy(self.component)
+
+                with ui.row().classes('w-full h-full'):
+                    with ui.column():
+                        ui.label('Shape:')
+                        ui.label(f'{self.array.shape}')
 
                 ui.separator()
 
-                table = ui.table.from_pandas(simultan_multi_value_big_table_to_pandas(self.component)
-                                             ).classes('w-full h-full')
+                self.table_ui_content()
 
-                with table.add_slot('top-left'):
-                    def toggle() -> None:
-                        table.toggle_fullscreen()
-                        button.props('icon=fullscreen_exit' if table.is_fullscreen else 'icon=fullscreen')
+                with ui.card().classes('w-full h-full'):
+                    ui.label('Select dimension to display:')
+                    self.dim_slider = ui.slider(min=0, max=self.array.shape[0] - 1,
+                                                step=1,
+                                                value=0,
+                                                on_change=self.table_ui_content.refresh)
+                    ui.input('dim_slider',
+                             value='0').bind_value(self.dim_slider,
+                                                   'value',
+                                                   forward=lambda x: int(x),
+                                                   backward=lambda x: str(x))
 
-                    button = ui.button('Toggle fullscreen', icon='fullscreen', on_click=toggle).props('flat')
+    @ui.refreshable
+    def table_ui_content(self):
 
+        if self.array.shape.__len__() > 2:
+            disp_array = self.array[int(self.dim_slider.value if self.dim_slider is not None else 0), :, :]
+        else:
+            disp_array = self.array
 
-class DataFrameManager(TypeViewManager):
+        self.table = ui.table.from_pandas(pd.DataFrame(disp_array),
+                                          ).classes('w-full h-full')
+        with self.table.add_slot('top-left'):
+            def toggle() -> None:
+                self.table.toggle_fullscreen()
+                button.props('icon=fullscreen_exit' if self.table.is_fullscreen else 'icon=fullscreen')
 
-    cls: pd.DataFrame = pd.DataFrame
-    item_view_cls: Type[TypeView] = DataFrameView
-    item_view_name = 'Dataframes'
+            button = ui.button('Toggle fullscreen', icon='fullscreen', on_click=toggle).props('flat')
 
-    def button_create_ui_content(self):
-        ui.button('Create new DataFrame', on_click=self.create_new_item, icon='add')
 
-    def update_items(self) -> list[SimMultiValueBigTable]:
+class NDArrayView(TypeView):
+
+    detail_view = NDArrayDetailView
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.content = kwargs.get('content', None)
+
+    @ui.refreshable
+    def ui_content(self):
+        from .detail_views import show_detail
+        with ui.card().classes(f"{self.colors['item']} w-full h-full") as self.card:
+            self.card.on('click', lambda e: show_detail(value=self.component,
+                                                        parent=self))
+            with ui.row().classes('bg-stone-100 w-full') as self.row:
+                self.row.on('click', lambda e: show_detail(value=self.component,
+                                                           parent=self))
+                self.checkbox = ui.checkbox(on_change=self.select)
+                ui.label(f'{self.component.Id}')
+                ui.label(f'{self.component.Name}')
+
+
+class NDArrayManager(TypeViewManager):
+
+    cls: np.ndarray = np.ndarray
+    item_view_cls: Type[TypeView] = NDArrayView
+    item_view_name = 'ND Arrays'
+
+    def update_items(self) -> list[SimMultiValueField3D]:
         if self.data_model is None:
             return []
+        return [x for x in self.data_model.value_fields if type(x) == SimMultiValueField3D]
 
-        return [x for x in self.data_model.value_fields if type(x) == SimMultiValueBigTable]
+    def button_create_ui_content(self):
+        ui.button('Create new ND-Array', on_click=self.create_new_item, icon='add')
 
     @ui.refreshable
     def add_item_to_view(self,
                          item: any,
                          raw_val=None):
 
-        if isinstance(item, SimMultiValueBigTable):
+        if isinstance(item, SimMultiValueField3D):
             val_source = item
-        elif isinstance(item, pd.DataFrame):
-            val_source: SimMultiValueBigTable = raw_val.ValueSource.ValueField
+        elif isinstance(item, np.ndarray):
+            val_source: SimMultiValueField3D = raw_val.ValueSource.ValueField
 
         if self.items_ui_element is None:
             return
 
         if val_source not in self.items:
             self.items.append(val_source)
         item_view = self.item_views.get(str(val_source.Id), None)
```

### Comparing `pysimultanui-0.1/src/views/parameter_view.py` & `pysimultanui-0.2/src/views/parameter_view.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.1/src/views/type_view.py` & `pysimultanui-0.2/src/views/type_view.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from typing import Optional
 from nicegui import ui, events
 from ..config import logger
 
-from . import view_manager
-from PySimultan2.simultan_object import SimultanObject
-from PySimultan2.files import FileInfo
-from ..core.edit_dialog import ContentEditDialog
-from .. import core
-
 
 class TypeView:
 
     colors = {'item': 'bg-stone-100',
               'cls_color': 'bg-stone-300',
               'selected': 'bg-blue-200'}
 
+    detail_view = None
+
     def __init__(self, *args, **kwargs) -> None:
 
         self._component = None
         self.checkbox = None
         self.component = kwargs.get('component', None)
         self.parent = kwargs.get('parent', None)
 
@@ -42,37 +38,29 @@
     def selected(self):
         if self.checkbox is None:
             return False
         return self.checkbox.value
 
     @ui.refreshable
     def ui_content(self):
+
+        from .detail_views import show_detail
+
         with ui.list().classes('w-full h-full') as self.card:
         # with ui.card().classes('w-full h-full').props('color="blue-800" keep-color') as self.card:
             with ui.item().classes('w-full h-full'):
                 with ui.item_section():
                     self.checkbox = ui.checkbox()
                 with ui.item_section():
                     ui.input(label='Name', value=self.component.name).bind_value(self.component, 'name')
                 with ui.item_section():
                     ui.label(f'{str(self.component.id)}')
                 with ui.item_section():
-                    ui.button(on_click=self.show_details, icon='open')
-
-    def show_details(self):
-        core.detail_view.clear()
-
-            # with ui.card().classes('w-full h-full').props('color="blue-800" keep-color') as self.card:
-            #     with ui.item().classes('w-full h-full'):
-            #         with ui.item_section():
-            #             self.checkbox = ui.checkbox()
-            #         with ui.item_section():
-            #             ui.input(label='Name', value=self.component.name).bind_value(self.component, 'name')
-            #         with ui.item_section():
-            #             ui.label(f'{str(self.component.id)}')
+                    ui.button(on_click=lambda e: show_detail(value=self.component,
+                                                             parent=self), icon='open')
 
     def select(self, e: events.ClickEventArguments):
         if self.selected:
             self.row.classes(remove=f"{self.colors['item']}", add=f"{self.colors['selected']}")
             self.card.classes(remove=f"{self.colors['item']}", add=f"{self.colors['selected']}")
         else:
             self.row.classes(add=f"{self.colors['item']}", remove=f"{self.colors['selected']}")
```

### Comparing `pysimultanui-0.1/src/views/type_view_manager.py` & `pysimultanui-0.2/src/views/type_view_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import os
 import shutil
 import asyncio
+from logging import getLogger
 from typing import Optional, Type
 
-from .. import core
+# from .. import core
+from .. import user_manager
 from nicegui import Client, app, ui, events
 from .type_view import TypeView
 from PySimultan2.simultan_object import SimultanObject
 
 
+logger = getLogger('py_simultan_ui')
+
+
 class TypeViewManager(object):
 
     cls: Optional[Type[SimultanObject]] = None
     item_view_cls: type[TypeView] = TypeView
     item_view_name = 'Item'
 
     def __init__(self, *args, **kwargs):
@@ -20,19 +25,35 @@
         self._data_model = None
         self._items = []
         self._item_views: dict[any, any] = {}
 
         self.items_ui_element = kwargs.get('items_ui_element', None)
         self.no_items_label = None
 
-        self.mapper = kwargs.get('mapper', core.mapper)
         self.data_model = kwargs.get('data_model', None)
         self.expansion: Optional[ui.expansion] = kwargs.get('expansion', None)
 
     @property
+    def project_manager(self):
+        return self.user.project_manager
+
+    @property
+    def mapper(self):
+        return self.user.mapper
+
+    @property
+    def user(self):
+        return user_manager[app.storage.user['username']]
+
+    @property
+    def taxonomy(self):
+        if self.cls is not None:
+            return self.cls._taxonomy if hasattr(self.cls, '_taxonomy') else self.cls
+
+    @property
     def items(self) -> list[any]:
         if self._items is None:
             self.items = self.update_items()
         return self._items
 
     @items.setter
     def items(self, value: list[any]):
@@ -60,33 +81,39 @@
 
     @property
     def selected_items(self):
         return [x for x in self.items if x.__ui_element__.selected]
 
     @data_model.setter
     def data_model(self, value):
+        logger.debug(f'View Manager setting data model to {value}')
         # self._item_views = {}
         self._data_model = value
         self._items = self.update_items()
         self.ui_content.refresh()
 
     @ui.refreshable
     def ui_content(self):
 
+        logger.info(f'Creating UI content for TVM {self.taxonomy}')
+
         with ui.expansion(icon='format_list_bulleted',
                           text=f'{self.item_view_name if self.item_view_name is not None else self.cls._taxonomy} '
                                f'({len(self.items)})'
                           ).classes('w-full h-full').bind_text_from(self,
                                                                     'items',
                                                                     lambda x: f'{self.item_view_name} ({len(x)})'
                                                                     ) as self.expansion:
             self.ui_expand_content()
 
     @ui.refreshable
     def ui_expand_content(self):
+
+        logger.info(f'Creating UI expand content for TVM {self.taxonomy}')
+
         self.items_ui_element = ui.row().classes('w-full h-full')
         with self.items_ui_element:
             if len(self.items) == 0:
                 with ui.item():
                     self.no_items_label = ui.label('No items to display')
 
         for item in self.items:
@@ -96,42 +123,50 @@
             self.button_create_ui_content()
 
     def button_create_ui_content(self):
         ui.button('Upload new Asset', on_click=self.create_new_item, icon='add')
 
     def update_items(self) -> list[any]:
 
+        logger.info(f'Updating items for TVM {self.taxonomy}')
+
         # return self.cls.cls_instances
 
         if self.cls is None:
             return []
-        mapped_cls = self.mapper.mapped_classes.get(self.cls._taxonomy, None)
+        mapped_cls = self.mapper.mapped_classes.get(self.taxonomy, None)
 
         if mapped_cls is None:
+            logger.warning(f'mapped_cls for TVM {self.taxonomy} is None!')
             return []
         if hasattr(mapped_cls, 'cls_instances'):
+            logger.info(f'Found {len(mapped_cls.cls_instances)} instances for TVM {self.taxonomy}')
             return mapped_cls.cls_instances
         return []
 
     def create_new_item(self, event):
 
+        logger.info(f'Updating items for TVM {self.taxonomy}')
+
         if self.data_model is None:
             ui.notify('No data model selected! Please load a data model first.')
             return
 
         new_item = self.cls()
         self.add_item_to_view(new_item)
 
     def update_expansion_text(self):
         if self.expansion is not None:
             self.expansion.text = f'{self.item_view_name if self.item_view_name is not None else self.cls._taxonomy} ' \
                                   f'({len(self.items)})'
 
     def add_item_to_view(self, item: any):
 
+        logger.info(f'Adding item to TVM {self.taxonomy} view: {item}')
+
         if self.items_ui_element is None:
             return
 
         if item not in self.items:
             self.items.append(item)
         item_view: TypeView = self.item_views.get(item, None)
 
@@ -147,14 +182,17 @@
                 with self.items_ui_element:
                     item_view.ui_content()
 
         self.update_expansion_text()
         return item_view
 
     def remove_item_from_view(self, item: any):
+
+        logger.info(f'Removing item from TVM {self.taxonomy} view: {item}')
+
         try:
             item_view = self.item_views.get(item, None)
             if item_view is not None:
                 self.items_ui_element.remove(item_view.card)
                 self.item_views.pop(item)
                 item.__ui_element__ = None
         except Exception as e:
@@ -172,14 +210,16 @@
                 pass
 
     def new_instance_created(self, instance: any):
         self.add_item_to_view(instance)
 
     def update_items_views(self):
 
+        logger.info(f'Updating item views for TVM {self.taxonomy}')
+
         self.item_views = {}
         for item in self.items:
             try:
                 item.__ui_element__ = None
             except Exception as e:
                 pass
```

### Comparing `pysimultanui-0.1/src/views/view_manager.py` & `pysimultanui-0.2/src/core/user.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,163 +1,165 @@
-import pandas as pd
-import asyncio
-import numpy as np
-from copy import copy
-from nicegui import ui, run
-from typing import Optional
+import os
+from typing import Union, Optional
 
-from .type_view_manager import TypeViewManager
-from .type_view import TypeView
-from .. import core
-from ..core import PythonMapper
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from .method_mapper import MethodMapper
+    from PySimultan2.data_model import DataModel
+    from PySimultan2.object_mapper import PythonMapper
 
-from .mapped_cls.mapped_cls_manager import MappedClsManager
-from .mapped_cls.mapped_cls_view import MappedClsView
+initial_user_name = os.environ.get('INITIAL_USER_NAME', 'admin')
+initial_user_email = os.environ.get('INITIAL_USER_EMAIL', 'example@test.de')
+initial_user_password = os.environ.get('INITIAL_USER_PASSWORD', 'admin')
 
 
-from .component_list_view.component_list_manager import ComponentListManager
-from .component_list_view.component_list_view import ComponentListView
+class Singleton(type):
+    _instances = {}
 
-from .component_dict_view import ComponentDictManager, ComponentDictView
+    def __call__(cls, *args, **kwargs):
+        if cls not in cls._instances:
+            cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
+        return cls._instances[cls]
 
-from .pandas_df_view import DataFrameView, DataFrameManager
-from .numpy_view import NDArrayView, NDArrayManager
 
-from PySimultan2.simultan_object import SimultanObject
+class DetailHistory:
+    def __init__(self):
+        self.detail_history = []
+        self.detail_history_index = 0
+        self.current_detail = None
 
+    def add_item(self, item):
+        if len(self.detail_history) > 0 and self.detail_history_index <= len(self.detail_history) -1:
+            self.detail_history = self.detail_history[:self.detail_history_index]
+            self.detail_history_index = len(self.detail_history)
 
-class ViewManager(object):
+        self.detail_history.append(item)
+        if len(self.detail_history) > 10:
+            self.detail_history.pop(0)
+            self.detail_history_index = len(self.detail_history)
+        self.current_detail = item
 
-    def __init__(self, *args, **kwargs):
-
-        self._data_model = None
-
-        self.mapper = kwargs.get('mapper', core.mapper)
-        self.cls_views: dict[str:TypeViewManager, str:TypeView] = {}
-        self.data_model = kwargs.get('data_model', None)
-        self.parent = kwargs.get('parent', None)
-
-    def register(self,
-                 cls: type,
-                 type_view: type[TypeView],
-                 item_view_manager: Optional[TypeViewManager] = None,):
-
-        self.cls_views[cls] = {'item_view_manager': item_view_manager, 'type_view': type_view}
-        cls.item_view_manager = item_view_manager
-        cls.type_view = type_view
-
-    @property
-    def data_model(self):
-        return self._data_model
-
-    @data_model.setter
-    def data_model(self, value):
-        self._data_model = value
-
-        for cls, cls_view_dict in self.cls_views.items():
-            item_view_manager = cls_view_dict.get('item_view_manager', None)
-            if item_view_manager is None:
-                continue
-            else:
-                item_view_manager.data_model = value
+    def get_current_detail(self):
+        return self.current_detail
 
-    def get_view(self, cls: type):
-        return self.cls_views[cls]
+    def get_previous_detail(self):
+        if self.detail_history_index > 0:
+            return self.detail_history[self.detail_history_index]
 
-    def create_mapped_cls_view_manager(self, taxonomy: str) -> Optional[TypeViewManager]:
-        cls = self.mapper.get_mapped_class(taxonomy)
+    def get_next_detail(self):
+        if self.detail_history_index < len(self.detail_history) - 1:
+            return self.detail_history[self.detail_history_index]
 
-        if self.cls_views.get(cls, None) is None:
-            new_tvm = MappedClsManager(mapper=self.mapper)
-            new_tvm.cls = self.mapper.get_mapped_class(taxonomy)
-            # old__init__ = copy(new_tvm.cls.__init__)
-            #
-            # def __init__(self, *args, **kwargs):
-            #     old__init__(self, *args, **kwargs)
-            #     new_tvm.add_item_to_view(self)
-            #
-            # new_tvm.cls.__init__ = __init__
+    def __len__(self):
+        return len(self.detail_history)
 
-            new_tvm.item_view_cls = MappedClsView
-            new_tvm.item_view_name = taxonomy
-            new_tvm.view_manager = self
-            self.cls_views[new_tvm.cls] = {'item_view_manager': new_tvm, 'type_view': MappedClsView}
+    def move_next(self):
+        if self.detail_history_index < len(self.detail_history) - 1:
+            self.detail_history_index += 1
+            return self.detail_history[self.detail_history_index]
 
-            with core.project_tab:
-                new_tvm.ui_content()
+    def move_previous(self):
+        if self.detail_history_index > 0:
+            self.detail_history_index -= 1
+            return self.detail_history[self.detail_history_index]
 
-        return self.cls_views.get(cls, None)
 
-    @ui.refreshable
-    def ui_content(self):
+class User:
 
-        core.method_mapper.ui_content()
+    def __init__(self, *args, **kwargs):
 
-        def add_new_init_method(tvm: TypeViewManager):
-            old__init__ = copy(tvm.cls.__init__)
+        from ..core import method_mapper, mapper
 
-            def __init__(self, *args, **kwargs):
-                old__init__(self, *args, **kwargs)
-                tvm.add_item_to_view(self)
+        self._project_manager = None
+        self._view_manager = None
+        self._asset_manager = None
+        self._geometry_manager = None
+        self._navigation = None
+
+        self.user_manager = kwargs.get('user_manager', None)
+
+        self.name = kwargs.get('name', None)
+        self.email = kwargs.get('email', None)
+        self.password = kwargs.get('password', None)
+
+        self.mapper: Optional[PythonMapper] = kwargs.get('mapper', mapper)
+        self.method_mapper: Optional[MethodMapper] = kwargs.get('method_mapper', method_mapper)
+        self.data_model: Union[DataModel, None] = kwargs.get('data_model', None)
+
+        self.navigation_drawer = kwargs.get('navigation_drawer', None)
+        self.project_tab = kwargs.get('navigation_drawer', None)
+        self.detail_view = kwargs.get('navigation_drawer', None)
+        self.home_tab = kwargs.get('navigation_drawer', None)
 
-            tvm.cls.__init__ = __init__
+        self.detail_history = DetailHistory()
 
-        for taxonomy, cls in self.mapper.registered_classes.items():
+    @property
+    def project_manager(self):
+        if self._project_manager is None:
+            from .project_manager import ProjectManager
+            self._project_manager = ProjectManager(user_manager=self.user_manager,
+                                                   mapper=self.mapper)
+        return self._project_manager
 
-            mapped_cls = self.mapper.get_mapped_class(taxonomy)
+    @property
+    def view_manager(self):
+        if self._view_manager is None:
+            from ..views.view_manager import ViewManager
+            self._view_manager = ViewManager(mapper=self.mapper,
+                                             parent=self.project_manager)
+        return self._view_manager
 
-            if taxonomy == 'ComponentList':
-                new_tvm = ComponentListManager(mapper=self.mapper)
-                new_tvm.item_view_cls = ComponentListView
+    @property
+    def asset_manager(self):
+        if self._asset_manager is None:
+            from ..views.asset_view import AssetManager
+            self._asset_manager = AssetManager()
+        return self._asset_manager
 
-            elif taxonomy == 'ComponentDict':
-                new_tvm = ComponentDictManager(mapper=self.mapper)
-                new_tvm.item_view_cls = ComponentDictView
+    @property
+    def geometry_manager(self):
+        if self._geometry_manager is None:
+            from ..views.geometry_view import GeometryManager
+            self._geometry_manager = GeometryManager(data_model=self.data_model)
+        return self._geometry_manager
 
-            elif self.cls_views.get(cls, None) is None:
-                new_tvm = MappedClsManager(mapper=self.mapper)
-                new_tvm.item_view_cls = MappedClsView
+    @property
+    def navigation(self):
+        if self._navigation is None:
+            from .navigation import Navigation
+            self._navigation = Navigation()
+        return self._navigation
 
-            else:
-                new_tvm = self.cls_views.get(cls, None)['item_view_manager']
 
-            if new_tvm is None:
-                continue
+class Admin(User):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
-            new_tvm.cls = mapped_cls
-            # add_new_init_method(new_tvm)
-            new_tvm.item_view_name = taxonomy
-            new_tvm.view_manager = self
-            self.cls_views[new_tvm.cls] = {'item_view_manager': new_tvm, 'type_view': new_tvm.item_view_cls}
-            new_tvm.ui_content()
 
-        df_manager = DataFrameManager(mapper=self.mapper)
-        self.cls_views[pd.DataFrame] = {'item_view_manager': df_manager, 'type_view': DataFrameView}
-        df_manager.ui_content()
+class UserManager(metaclass=Singleton):
 
-        np_manager = NDArrayManager(mapper=self.mapper)
-        self.cls_views[np.ndarray] = {'item_view_manager': np_manager, 'type_view': NDArrayView}
-        np_manager.ui_content()
+    def __init__(self):
+        self.users = {}
+        self.create_initial_users()
 
-    async def refresh_all_items(self):
+    def create_initial_users(self):
+        admin = Admin(name=initial_user_name,
+                      email=initial_user_email,
+                      password=initial_user_password,
+                      user_manager=self)
 
-        n = ui.notification(timeout=None)
-        n.spinner = True
-        n.message = 'Updating all items...'
+        self.users[initial_user_name] = admin
 
-        for tvm_dict in self.cls_views.values():
-            tvm: Optional[TypeViewManager, None] = tvm_dict.get('item_view_manager', None)
-            if tvm is None:
-                continue
-            print(f'Updating items of {tvm.item_view_name}...')
-            n.message = f'Updating items of {tvm.item_view_name}...'
-            tvm.update_items_views()
+        user_1 = User(name=initial_user_name + '_2',
+                      email=initial_user_email + '_2',
+                      password=initial_user_password + '_2',
+                      user_manager=self)
 
-        ui.notify('All items updated!', type='positive')
+        self.users[initial_user_name + '_2'] = user_1
 
-        n.message = 'Updating all items done!'
-        n.type = 'positive'
-        n.spinner = False
-        await asyncio.sleep(2)
+    def authenticate(self, username, password):
+        if username in self.users and self.users[username].password == password:
+            return True
+        return False
 
-        # self.method(*args, **kwargs)
-        n.dismiss()
+    def __getitem__(self, key):
+        return self.users[key]
```

### Comparing `pysimultanui-0.1/tests/test_py_simultan_ui.py` & `pysimultanui-0.2/tests/test_py_simultan_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -642,8 +642,8 @@
                                   kwargs={})
 
 
 init_project()
 map_methods()
 run_ui()
 
-print('Test passed 48 47 1')
+print('Test passed 48 47 2')
```

