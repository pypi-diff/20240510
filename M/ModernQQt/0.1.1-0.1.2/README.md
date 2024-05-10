# Comparing `tmp/modernqqt-0.1.1.tar.gz` & `tmp/modernqqt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modernqqt-0.1.1.tar", max compression
+gzip compressed data, was "modernqqt-0.1.2.tar", max compression
```

## Comparing `modernqqt-0.1.1.tar` & `modernqqt-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 modernqqt-0.1.1/LICENSE
--rw-r--r--   0        0        0      920 2024-05-10 14:57:31.479942 modernqqt-0.1.1/README.md
--rw-r--r--   0        0        0       32 2024-05-10 14:50:59.291367 modernqqt-0.1.1/modernqqt/__init__.py
--rw-r--r--   0        0        0       79 2024-05-10 13:11:25.993250 modernqqt-0.1.1/modernqqt/src/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-10 13:11:26.243238 modernqqt-0.1.1/modernqqt/src/core/dialog.py
--rw-r--r--   0        0        0      101 2024-05-10 13:11:26.243238 modernqqt-0.1.1/modernqqt/src/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-10 13:11:26.243238 modernqqt-0.1.1/modernqqt/src/core/font.py
--rw-r--r--   0        0        0      324 2024-05-10 13:11:26.246571 modernqqt-0.1.1/modernqqt/src/core/load.py
--rw-r--r--   0        0        0     5387 2024-05-10 13:11:26.246571 modernqqt-0.1.1/modernqqt/src/ui/angle-down.png
--rw-r--r--   0        0        0      336 2024-05-10 13:11:26.246571 modernqqt-0.1.1/modernqqt/src/ui/angle-down.svg
--rw-r--r--   0        0        0      238 2024-05-10 13:11:26.249904 modernqqt-0.1.1/modernqqt/widgets/__init__.py
--rw-r--r--   0        0        0     1317 2024-05-10 14:50:59.291367 modernqqt-0.1.1/modernqqt/widgets/basic/button.py
--rw-r--r--   0        0        0      960 2024-05-10 14:50:59.291367 modernqqt-0.1.1/modernqqt/widgets/basic/groups.py
--rw-r--r--   0        0        0      993 2024-05-10 14:50:59.294700 modernqqt-0.1.1/modernqqt/widgets/basic/label.py
--rw-r--r--   0        0        0      278 2024-05-10 13:11:26.319901 modernqqt-0.1.1/modernqqt/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      501 2024-05-10 13:11:26.319901 modernqqt-0.1.1/modernqqt/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0      262 2024-05-10 13:11:26.323234 modernqqt-0.1.1/modernqqt/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      513 2024-05-10 13:11:26.323234 modernqqt-0.1.1/modernqqt/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0      286 2024-05-10 13:11:26.326568 modernqqt-0.1.1/modernqqt/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0      134 2024-05-10 13:11:26.326568 modernqqt-0.1.1/modernqqt/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0      265 2024-05-10 13:11:26.326568 modernqqt-0.1.1/modernqqt/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0      313 2024-05-10 13:11:26.329901 modernqqt-0.1.1/modernqqt/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0    10088 2024-05-10 14:50:59.294700 modernqqt-0.1.1/modernqqt/widgets/basic/switchers.py
--rw-r--r--   0        0        0     1578 2024-05-10 14:50:59.294700 modernqqt-0.1.1/modernqqt/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0      583 2024-05-10 14:58:35.147006 modernqqt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1615 1970-01-01 00:00:00.000000 modernqqt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 modernqqt-0.1.2/LICENSE
+-rw-r--r--   0        0        0      924 2024-05-10 15:57:38.790500 modernqqt-0.1.2/README.md
+-rw-r--r--   0        0        0      320 2024-05-10 15:43:30.031280 modernqqt-0.1.2/modernqqt/__init__.py
+-rw-r--r--   0        0        0       79 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/src/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/src/core/dialog.py
+-rw-r--r--   0        0        0      101 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/src/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/src/core/font.py
+-rw-r--r--   0        0        0      324 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/src/core/load.py
+-rw-r--r--   0        0        0     5387 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/src/ui/angle-down.png
+-rw-r--r--   0        0        0      336 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/src/ui/angle-down.svg
+-rw-r--r--   0        0        0      238 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/__init__.py
+-rw-r--r--   0        0        0     1317 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/button.py
+-rw-r--r--   0        0        0      960 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/groups.py
+-rw-r--r--   0        0        0      993 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/label.py
+-rw-r--r--   0        0        0      278 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      501 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0      262 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      513 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0      286 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0      134 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0      265 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0      313 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0    10088 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/switchers.py
+-rw-r--r--   0        0        0     1578 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0      602 2024-05-10 15:58:58.953623 modernqqt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 modernqqt-0.1.2/PKG-INFO
```

### Comparing `modernqqt-0.1.1/LICENSE` & `modernqqt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.1/README.md` & `modernqqt-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,18 @@
     <img src="Logo.png">
 </p>
 <h1></h1>
 
 <p align="center">
 
   <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/ModernQQt">
-  <img src="https://img.shields.io/github/license/chebupelka8/ModernQt">
-  <img src="https://img.shields.io/github/commit-activity/t/chebupelka8/ModernQt"> 
-  <img src="https://img.shields.io/github/stars/chebupelka8/ModernQt">
-  <img src="https://img.shields.io/github/watchers/chebupelka8/ModernQt">
+  <img src="https://img.shields.io/github/license/chebupelka8/ModernQQt">
+  <img src="https://img.shields.io/github/commit-activity/t/chebupelka8/ModernQQt"> 
+  <img src="https://img.shields.io/github/stars/chebupelka8/ModernQQt">
+  <img src="https://img.shields.io/github/watchers/chebupelka8/ModernQQt">
   
 </p>
 
 <b>ModernQt</b>: A Cutting-Edge GUI Library Built on PyQt6 ModernQt is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now ModernQt is in development.
 
 <h3>How to use</h3>
```

### Comparing `modernqqt-0.1.1/modernqqt/src/core/dialog.py` & `modernqqt-0.1.2/modernqqt/src/core/dialog.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.1/modernqqt/src/core/font.py` & `modernqqt-0.1.2/modernqqt/src/core/font.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.1/modernqqt/src/ui/angle-down.png` & `modernqqt-0.1.2/modernqqt/src/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.1/modernqqt/widgets/basic/button.py` & `modernqqt-0.1.2/modernqqt/widgets/basic/button.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.1/modernqqt/widgets/basic/groups.py` & `modernqqt-0.1.2/modernqqt/widgets/basic/groups.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.1/modernqqt/widgets/basic/label.py` & `modernqqt-0.1.2/modernqqt/widgets/basic/label.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.1/modernqqt/widgets/basic/styles/drop_down_menu.css` & `modernqqt-0.1.2/modernqqt/widgets/basic/styles/drop_down_menu.css`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.1/modernqqt/widgets/basic/switchers.py` & `modernqqt-0.1.2/modernqqt/widgets/basic/switchers.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.1/modernqqt/widgets/basic/widgets_list.py` & `modernqqt-0.1.2/modernqqt/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.1/pyproject.toml` & `modernqqt-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "ModernQQt"
-version = "0.1.1"
+version = "0.1.2"
 description = "ModernQt: A Cutting-Edge GUI Library Built on PyQt6 ModernQt is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now ModernQt is in development."
 authors = ["chebupelka8 <stpzamyatin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
+pyside6 = "^6.7.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `modernqqt-0.1.1/PKG-INFO` & `modernqqt-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: ModernQQt
-Version: 0.1.1
+Version: 0.1.2
 Summary: ModernQt: A Cutting-Edge GUI Library Built on PyQt6 ModernQt is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now ModernQt is in development.
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pyside6 (>=6.7.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
     <img src="Logo.png">
 </p>
 <h1></h1>
 
 <p align="center">
 
   <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/ModernQQt">
-  <img src="https://img.shields.io/github/license/chebupelka8/ModernQt">
-  <img src="https://img.shields.io/github/commit-activity/t/chebupelka8/ModernQt"> 
-  <img src="https://img.shields.io/github/stars/chebupelka8/ModernQt">
-  <img src="https://img.shields.io/github/watchers/chebupelka8/ModernQt">
+  <img src="https://img.shields.io/github/license/chebupelka8/ModernQQt">
+  <img src="https://img.shields.io/github/commit-activity/t/chebupelka8/ModernQQt"> 
+  <img src="https://img.shields.io/github/stars/chebupelka8/ModernQQt">
+  <img src="https://img.shields.io/github/watchers/chebupelka8/ModernQQt">
   
 </p>
 
 <b>ModernQt</b>: A Cutting-Edge GUI Library Built on PyQt6 ModernQt is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now ModernQt is in development.
 
 <h3>How to use</h3>
```

