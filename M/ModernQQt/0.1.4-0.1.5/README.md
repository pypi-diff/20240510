# Comparing `tmp/modernqqt-0.1.4.tar.gz` & `tmp/modernqqt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modernqqt-0.1.4.tar", max compression
+gzip compressed data, was "modernqqt-0.1.5.tar", max compression
```

## Comparing `modernqqt-0.1.4.tar` & `modernqqt-0.1.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 modernqqt-0.1.4/LICENSE
--rw-r--r--   0        0        0     1296 2024-05-10 17:14:41.467165 modernqqt-0.1.4/README.md
--rw-r--r--   0        0        0      320 2024-05-10 15:43:30.031280 modernqqt-0.1.4/modernqqt/__init__.py
--rw-r--r--   0        0        0       38 2024-05-10 16:49:32.417643 modernqqt-0.1.4/modernqqt/constructor/__init__.py
--rw-r--r--   0        0        0      552 2024-05-10 17:10:15.186165 modernqqt-0.1.4/modernqqt/constructor/initialize.py
--rw-r--r--   0        0        0    12449 2024-05-10 17:57:00.224042 modernqqt-0.1.4/modernqqt/resources/Icon.png
--rw-r--r--   0        0        0    17677 2024-05-10 17:57:00.227375 modernqqt-0.1.4/modernqqt/resources/Logo.png
--rw-r--r--   0        0        0        0 2024-05-10 17:57:00.227375 modernqqt-0.1.4/modernqqt/resources/__init__.py
--rw-r--r--   0        0        0     5387 2024-05-10 17:57:00.227375 modernqqt-0.1.4/modernqqt/resources/ui/angle-down.png
--rw-r--r--   0        0        0      336 2024-05-10 17:57:00.227375 modernqqt-0.1.4/modernqqt/resources/ui/angle-down.svg
--rw-r--r--   0        0        0      120 2024-05-10 17:10:15.186165 modernqqt-0.1.4/modernqqt/src/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-10 14:59:21.961513 modernqqt-0.1.4/modernqqt/src/core/dialog.py
--rw-r--r--   0        0        0      151 2024-05-10 17:10:15.186165 modernqqt-0.1.4/modernqqt/src/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-10 14:59:21.961513 modernqqt-0.1.4/modernqqt/src/core/font.py
--rw-r--r--   0        0        0      324 2024-05-10 14:59:21.961513 modernqqt-0.1.4/modernqqt/src/core/load.py
--rw-r--r--   0        0        0      589 2024-05-10 17:10:15.186165 modernqqt-0.1.4/modernqqt/src/core/stylesheet.py
--rw-r--r--   0        0        0       22 2024-05-10 17:57:00.227375 modernqqt-0.1.4/modernqqt/src/util/__init__.py
--rw-r--r--   0        0        0      125 2024-05-10 17:57:00.227375 modernqqt-0.1.4/modernqqt/src/util/config.py
--rw-r--r--   0        0        0      238 2024-05-10 14:59:21.961513 modernqqt-0.1.4/modernqqt/widgets/__init__.py
--rw-r--r--   0        0        0     1167 2024-05-10 17:10:15.186165 modernqqt-0.1.4/modernqqt/widgets/basic/button.py
--rw-r--r--   0        0        0      809 2024-05-10 17:10:15.186165 modernqqt-0.1.4/modernqqt/widgets/basic/groups.py
--rw-r--r--   0        0        0      993 2024-05-10 14:59:21.961513 modernqqt-0.1.4/modernqqt/widgets/basic/label.py
--rw-r--r--   0        0        0      278 2024-05-10 14:59:21.961513 modernqqt-0.1.4/modernqqt/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      501 2024-05-10 14:59:21.961513 modernqqt-0.1.4/modernqqt/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0      262 2024-05-10 14:59:21.961513 modernqqt-0.1.4/modernqqt/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      535 2024-05-10 17:57:00.227375 modernqqt-0.1.4/modernqqt/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0      286 2024-05-10 14:59:21.961513 modernqqt-0.1.4/modernqqt/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0      134 2024-05-10 14:59:21.961513 modernqqt-0.1.4/modernqqt/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0      265 2024-05-10 14:59:21.961513 modernqqt-0.1.4/modernqqt/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0      313 2024-05-10 14:59:21.961513 modernqqt-0.1.4/modernqqt/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0     9395 2024-05-10 17:57:00.227375 modernqqt-0.1.4/modernqqt/widgets/basic/switchers.py
--rw-r--r--   0        0        0     1578 2024-05-10 14:59:21.961513 modernqqt-0.1.4/modernqqt/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0       36 2024-05-10 16:49:32.417643 modernqqt-0.1.4/modernqqt/windows/__init__.py
--rw-r--r--   0        0        0     1139 2024-05-10 17:10:15.186165 modernqqt-0.1.4/modernqqt/windows/main_window.py
--rw-r--r--   0        0        0       58 2024-05-10 17:10:15.186165 modernqqt-0.1.4/modernqqt/windows/styles/main_window.css
--rw-r--r--   0        0        0      602 2024-05-10 17:57:00.227375 modernqqt-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2031 1970-01-01 00:00:00.000000 modernqqt-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 modernqqt-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1296 2024-05-10 17:14:41.467165 modernqqt-0.1.5/README.md
+-rw-r--r--   0        0        0      320 2024-05-10 15:43:30.031280 modernqqt-0.1.5/modernqqt/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-10 16:49:32.417643 modernqqt-0.1.5/modernqqt/constructor/__init__.py
+-rw-r--r--   0        0        0      552 2024-05-10 17:10:15.186165 modernqqt-0.1.5/modernqqt/constructor/initialize.py
+-rw-r--r--   0        0        0    12449 2024-05-10 17:57:00.224042 modernqqt-0.1.5/modernqqt/resources/Icon.png
+-rw-r--r--   0        0        0    17677 2024-05-10 17:57:00.227375 modernqqt-0.1.5/modernqqt/resources/Logo.png
+-rw-r--r--   0        0        0        0 2024-05-10 17:57:00.227375 modernqqt-0.1.5/modernqqt/resources/__init__.py
+-rw-r--r--   0        0        0     5387 2024-05-10 17:57:00.227375 modernqqt-0.1.5/modernqqt/resources/ui/angle-down.png
+-rw-r--r--   0        0        0      336 2024-05-10 17:57:00.227375 modernqqt-0.1.5/modernqqt/resources/ui/angle-down.svg
+-rw-r--r--   0        0        0      120 2024-05-10 17:10:15.186165 modernqqt-0.1.5/modernqqt/src/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-10 14:59:21.961513 modernqqt-0.1.5/modernqqt/src/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-10 17:10:15.186165 modernqqt-0.1.5/modernqqt/src/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-10 14:59:21.961513 modernqqt-0.1.5/modernqqt/src/core/font.py
+-rw-r--r--   0        0        0      324 2024-05-10 14:59:21.961513 modernqqt-0.1.5/modernqqt/src/core/load.py
+-rw-r--r--   0        0        0      589 2024-05-10 17:10:15.186165 modernqqt-0.1.5/modernqqt/src/core/stylesheet.py
+-rw-r--r--   0        0        0       22 2024-05-10 17:57:00.227375 modernqqt-0.1.5/modernqqt/src/util/__init__.py
+-rw-r--r--   0        0        0      125 2024-05-10 17:57:00.227375 modernqqt-0.1.5/modernqqt/src/util/config.py
+-rw-r--r--   0        0        0      238 2024-05-10 14:59:21.961513 modernqqt-0.1.5/modernqqt/widgets/__init__.py
+-rw-r--r--   0        0        0     1167 2024-05-10 17:10:15.186165 modernqqt-0.1.5/modernqqt/widgets/basic/button.py
+-rw-r--r--   0        0        0      809 2024-05-10 17:10:15.186165 modernqqt-0.1.5/modernqqt/widgets/basic/groups.py
+-rw-r--r--   0        0        0      993 2024-05-10 14:59:21.961513 modernqqt-0.1.5/modernqqt/widgets/basic/label.py
+-rw-r--r--   0        0        0      278 2024-05-10 14:59:21.961513 modernqqt-0.1.5/modernqqt/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      501 2024-05-10 14:59:21.961513 modernqqt-0.1.5/modernqqt/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0      293 2024-05-10 18:11:50.851226 modernqqt-0.1.5/modernqqt/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      474 2024-05-10 18:12:12.410288 modernqqt-0.1.5/modernqqt/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0      286 2024-05-10 14:59:21.961513 modernqqt-0.1.5/modernqqt/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0      134 2024-05-10 14:59:21.961513 modernqqt-0.1.5/modernqqt/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0      265 2024-05-10 14:59:21.961513 modernqqt-0.1.5/modernqqt/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0      313 2024-05-10 14:59:21.961513 modernqqt-0.1.5/modernqqt/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0     9395 2024-05-10 17:57:00.227375 modernqqt-0.1.5/modernqqt/widgets/basic/switchers.py
+-rw-r--r--   0        0        0     1578 2024-05-10 14:59:21.961513 modernqqt-0.1.5/modernqqt/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0       36 2024-05-10 16:49:32.417643 modernqqt-0.1.5/modernqqt/windows/__init__.py
+-rw-r--r--   0        0        0     1139 2024-05-10 17:10:15.186165 modernqqt-0.1.5/modernqqt/windows/main_window.py
+-rw-r--r--   0        0        0       58 2024-05-10 17:10:15.186165 modernqqt-0.1.5/modernqqt/windows/styles/main_window.css
+-rw-r--r--   0        0        0      602 2024-05-10 18:12:34.306001 modernqqt-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2031 1970-01-01 00:00:00.000000 modernqqt-0.1.5/PKG-INFO
```

### Comparing `modernqqt-0.1.4/LICENSE` & `modernqqt-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.4/README.md` & `modernqqt-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.4/modernqqt/constructor/initialize.py` & `modernqqt-0.1.5/modernqqt/constructor/initialize.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.4/modernqqt/resources/Icon.png` & `modernqqt-0.1.5/modernqqt/resources/Icon.png`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.4/modernqqt/resources/Logo.png` & `modernqqt-0.1.5/modernqqt/resources/Logo.png`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.4/modernqqt/resources/ui/angle-down.png` & `modernqqt-0.1.5/modernqqt/resources/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.4/modernqqt/src/core/dialog.py` & `modernqqt-0.1.5/modernqqt/src/core/dialog.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.4/modernqqt/src/core/font.py` & `modernqqt-0.1.5/modernqqt/src/core/font.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.4/modernqqt/src/core/stylesheet.py` & `modernqqt-0.1.5/modernqqt/src/core/stylesheet.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.4/modernqqt/widgets/basic/button.py` & `modernqqt-0.1.5/modernqqt/widgets/basic/button.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.4/modernqqt/widgets/basic/groups.py` & `modernqqt-0.1.5/modernqqt/widgets/basic/groups.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.4/modernqqt/widgets/basic/label.py` & `modernqqt-0.1.5/modernqqt/widgets/basic/label.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.4/modernqqt/widgets/basic/switchers.py` & `modernqqt-0.1.5/modernqqt/widgets/basic/switchers.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.4/modernqqt/widgets/basic/widgets_list.py` & `modernqqt-0.1.5/modernqqt/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.4/modernqqt/windows/main_window.py` & `modernqqt-0.1.5/modernqqt/windows/main_window.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.4/pyproject.toml` & `modernqqt-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ModernQQt"
-version = "0.1.4"
+version = "0.1.5"
 description = "ModernQt: A Cutting-Edge GUI Library Built on PyQt6 ModernQt is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now ModernQt is in development."
 authors = ["chebupelka8 <stpzamyatin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `modernqqt-0.1.4/PKG-INFO` & `modernqqt-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ModernQQt
-Version: 0.1.4
+Version: 0.1.5
 Summary: ModernQt: A Cutting-Edge GUI Library Built on PyQt6 ModernQt is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now ModernQt is in development.
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

