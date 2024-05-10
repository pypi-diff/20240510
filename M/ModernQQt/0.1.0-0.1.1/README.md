# Comparing `tmp/modernqqt-0.1.0.tar.gz` & `tmp/modernqqt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modernqqt-0.1.0.tar", max compression
+gzip compressed data, was "modernqqt-0.1.1.tar", max compression
```

## Comparing `modernqqt-0.1.0.tar` & `modernqqt-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 modernqqt-0.1.0/LICENSE
--rw-r--r--   0        0        0      917 2024-05-10 11:43:54.426363 modernqqt-0.1.0/README.md
--rw-r--r--   0        0        0       32 2024-05-10 14:50:59.291367 modernqqt-0.1.0/modernqqt/__init__.py
--rw-r--r--   0        0        0       79 2024-05-10 13:11:25.993250 modernqqt-0.1.0/modernqqt/src/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-10 13:11:26.243238 modernqqt-0.1.0/modernqqt/src/core/dialog.py
--rw-r--r--   0        0        0      101 2024-05-10 13:11:26.243238 modernqqt-0.1.0/modernqqt/src/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-10 13:11:26.243238 modernqqt-0.1.0/modernqqt/src/core/font.py
--rw-r--r--   0        0        0      324 2024-05-10 13:11:26.246571 modernqqt-0.1.0/modernqqt/src/core/load.py
--rw-r--r--   0        0        0     5387 2024-05-10 13:11:26.246571 modernqqt-0.1.0/modernqqt/src/ui/angle-down.png
--rw-r--r--   0        0        0      336 2024-05-10 13:11:26.246571 modernqqt-0.1.0/modernqqt/src/ui/angle-down.svg
--rw-r--r--   0        0        0      238 2024-05-10 13:11:26.249904 modernqqt-0.1.0/modernqqt/widgets/__init__.py
--rw-r--r--   0        0        0     1317 2024-05-10 14:50:59.291367 modernqqt-0.1.0/modernqqt/widgets/basic/button.py
--rw-r--r--   0        0        0      960 2024-05-10 14:50:59.291367 modernqqt-0.1.0/modernqqt/widgets/basic/groups.py
--rw-r--r--   0        0        0      993 2024-05-10 14:50:59.294700 modernqqt-0.1.0/modernqqt/widgets/basic/label.py
--rw-r--r--   0        0        0      278 2024-05-10 13:11:26.319901 modernqqt-0.1.0/modernqqt/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      501 2024-05-10 13:11:26.319901 modernqqt-0.1.0/modernqqt/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0      262 2024-05-10 13:11:26.323234 modernqqt-0.1.0/modernqqt/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      513 2024-05-10 13:11:26.323234 modernqqt-0.1.0/modernqqt/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0      286 2024-05-10 13:11:26.326568 modernqqt-0.1.0/modernqqt/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0      134 2024-05-10 13:11:26.326568 modernqqt-0.1.0/modernqqt/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0      265 2024-05-10 13:11:26.326568 modernqqt-0.1.0/modernqqt/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0      313 2024-05-10 13:11:26.329901 modernqqt-0.1.0/modernqqt/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0    10088 2024-05-10 14:50:59.294700 modernqqt-0.1.0/modernqqt/widgets/basic/switchers.py
--rw-r--r--   0        0        0     1578 2024-05-10 14:50:59.294700 modernqqt-0.1.0/modernqqt/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0      583 2024-05-10 14:50:32.619264 modernqqt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1612 1970-01-01 00:00:00.000000 modernqqt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 modernqqt-0.1.1/LICENSE
+-rw-r--r--   0        0        0      920 2024-05-10 14:57:31.479942 modernqqt-0.1.1/README.md
+-rw-r--r--   0        0        0       32 2024-05-10 14:50:59.291367 modernqqt-0.1.1/modernqqt/__init__.py
+-rw-r--r--   0        0        0       79 2024-05-10 13:11:25.993250 modernqqt-0.1.1/modernqqt/src/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-10 13:11:26.243238 modernqqt-0.1.1/modernqqt/src/core/dialog.py
+-rw-r--r--   0        0        0      101 2024-05-10 13:11:26.243238 modernqqt-0.1.1/modernqqt/src/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-10 13:11:26.243238 modernqqt-0.1.1/modernqqt/src/core/font.py
+-rw-r--r--   0        0        0      324 2024-05-10 13:11:26.246571 modernqqt-0.1.1/modernqqt/src/core/load.py
+-rw-r--r--   0        0        0     5387 2024-05-10 13:11:26.246571 modernqqt-0.1.1/modernqqt/src/ui/angle-down.png
+-rw-r--r--   0        0        0      336 2024-05-10 13:11:26.246571 modernqqt-0.1.1/modernqqt/src/ui/angle-down.svg
+-rw-r--r--   0        0        0      238 2024-05-10 13:11:26.249904 modernqqt-0.1.1/modernqqt/widgets/__init__.py
+-rw-r--r--   0        0        0     1317 2024-05-10 14:50:59.291367 modernqqt-0.1.1/modernqqt/widgets/basic/button.py
+-rw-r--r--   0        0        0      960 2024-05-10 14:50:59.291367 modernqqt-0.1.1/modernqqt/widgets/basic/groups.py
+-rw-r--r--   0        0        0      993 2024-05-10 14:50:59.294700 modernqqt-0.1.1/modernqqt/widgets/basic/label.py
+-rw-r--r--   0        0        0      278 2024-05-10 13:11:26.319901 modernqqt-0.1.1/modernqqt/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      501 2024-05-10 13:11:26.319901 modernqqt-0.1.1/modernqqt/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0      262 2024-05-10 13:11:26.323234 modernqqt-0.1.1/modernqqt/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      513 2024-05-10 13:11:26.323234 modernqqt-0.1.1/modernqqt/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0      286 2024-05-10 13:11:26.326568 modernqqt-0.1.1/modernqqt/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0      134 2024-05-10 13:11:26.326568 modernqqt-0.1.1/modernqqt/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0      265 2024-05-10 13:11:26.326568 modernqqt-0.1.1/modernqqt/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0      313 2024-05-10 13:11:26.329901 modernqqt-0.1.1/modernqqt/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0    10088 2024-05-10 14:50:59.294700 modernqqt-0.1.1/modernqqt/widgets/basic/switchers.py
+-rw-r--r--   0        0        0     1578 2024-05-10 14:50:59.294700 modernqqt-0.1.1/modernqqt/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0      583 2024-05-10 14:58:35.147006 modernqqt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1615 1970-01-01 00:00:00.000000 modernqqt-0.1.1/PKG-INFO
```

### Comparing `modernqqt-0.1.0/LICENSE` & `modernqqt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.0/README.md` & `modernqqt-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 <p align="center">
     <img src="Logo.png">
 </p>
 <h1></h1>
 
 <p align="center">
 
-  <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/ModernQt">
+  <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/ModernQQt">
   <img src="https://img.shields.io/github/license/chebupelka8/ModernQt">
   <img src="https://img.shields.io/github/commit-activity/t/chebupelka8/ModernQt"> 
   <img src="https://img.shields.io/github/stars/chebupelka8/ModernQt">
   <img src="https://img.shields.io/github/watchers/chebupelka8/ModernQt">
   
 </p>
 
 <b>ModernQt</b>: A Cutting-Edge GUI Library Built on PyQt6 ModernQt is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now ModernQt is in development.
 
 <h3>How to use</h3>
 
 ```sh
-pip install ModernQt
+pip install ModernQQt
 ```
 
 ```python
-from ModernQt.widgets import PushButton
+from modernqqt.widgets import PushButton
 ...
 ```
 
 <h3>Example</h3>
 <img src="example.png">
```

### Comparing `modernqqt-0.1.0/modernqqt/src/core/dialog.py` & `modernqqt-0.1.1/modernqqt/src/core/dialog.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.0/modernqqt/src/core/font.py` & `modernqqt-0.1.1/modernqqt/src/core/font.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.0/modernqqt/src/ui/angle-down.png` & `modernqqt-0.1.1/modernqqt/src/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.0/modernqqt/widgets/basic/button.py` & `modernqqt-0.1.1/modernqqt/widgets/basic/button.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.0/modernqqt/widgets/basic/groups.py` & `modernqqt-0.1.1/modernqqt/widgets/basic/groups.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.0/modernqqt/widgets/basic/label.py` & `modernqqt-0.1.1/modernqqt/widgets/basic/label.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.0/modernqqt/widgets/basic/styles/drop_down_menu.css` & `modernqqt-0.1.1/modernqqt/widgets/basic/styles/drop_down_menu.css`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.0/modernqqt/widgets/basic/switchers.py` & `modernqqt-0.1.1/modernqqt/widgets/basic/switchers.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.0/modernqqt/widgets/basic/widgets_list.py` & `modernqqt-0.1.1/modernqqt/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.0/pyproject.toml` & `modernqqt-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ModernQQt"
-version = "0.1.0"
+version = "0.1.1"
 description = "ModernQt: A Cutting-Edge GUI Library Built on PyQt6 ModernQt is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now ModernQt is in development."
 authors = ["chebupelka8 <stpzamyatin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `modernqqt-0.1.0/PKG-INFO` & `modernqqt-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ModernQQt
-Version: 0.1.0
+Version: 0.1.1
 Summary: ModernQt: A Cutting-Edge GUI Library Built on PyQt6 ModernQt is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now ModernQt is in development.
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,31 +15,31 @@
 <p align="center">
     <img src="Logo.png">
 </p>
 <h1></h1>
 
 <p align="center">
 
-  <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/ModernQt">
+  <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/ModernQQt">
   <img src="https://img.shields.io/github/license/chebupelka8/ModernQt">
   <img src="https://img.shields.io/github/commit-activity/t/chebupelka8/ModernQt"> 
   <img src="https://img.shields.io/github/stars/chebupelka8/ModernQt">
   <img src="https://img.shields.io/github/watchers/chebupelka8/ModernQt">
   
 </p>
 
 <b>ModernQt</b>: A Cutting-Edge GUI Library Built on PyQt6 ModernQt is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now ModernQt is in development.
 
 <h3>How to use</h3>
 
 ```sh
-pip install ModernQt
+pip install ModernQQt
 ```
 
 ```python
-from ModernQt.widgets import PushButton
+from modernqqt.widgets import PushButton
 ...
 ```
 
 <h3>Example</h3>
 <img src="example.png">
```

