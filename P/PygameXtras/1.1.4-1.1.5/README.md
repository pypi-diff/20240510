# Comparing `tmp/pygamextras-1.1.4.tar.gz` & `tmp/pygamextras-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygamextras-1.1.4.tar", max compression
+gzip compressed data, was "pygamextras-1.1.5.tar", max compression
```

## Comparing `pygamextras-1.1.4.tar` & `pygamextras-1.1.5.tar`

### file list

```diff
@@ -1,36 +1,39 @@
--rw-r--r--   0        0        0     1091 2023-09-24 01:46:21.865382 pygamextras-1.1.4/LICENSE.txt
--rw-r--r--   0        0        0       28 2023-09-23 15:29:20.709795 pygamextras-1.1.4/main/PygameXtras/__init__.py
--rw-r--r--   0        0        0        0 2023-09-23 16:11:25.887474 pygamextras-1.1.4/main/PygameXtras/src/__init__.py
--rw-r--r--   0        0        0      720 2023-11-04 14:00:58.396381 pygamextras-1.1.4/main/PygameXtras/src/classes/__init__.py
--rw-r--r--   0        0        0     9617 2023-11-25 20:44:04.832441 pygamextras-1.1.4/main/PygameXtras/src/classes/Bar.py
--rw-r--r--   0        0        0     3900 2023-09-23 15:53:12.120929 pygamextras-1.1.4/main/PygameXtras/src/classes/Button.py
--rw-r--r--   0        0        0     5619 2024-02-16 00:21:58.561099 pygamextras-1.1.4/main/PygameXtras/src/classes/C.py
--rw-r--r--   0        0        0    12895 2023-04-21 00:07:14.084627 pygamextras-1.1.4/main/PygameXtras/src/classes/Colors.py
--rw-r--r--   0        0        0     2555 2023-11-25 20:46:23.639451 pygamextras-1.1.4/main/PygameXtras/src/classes/CustomTemplate.py
--rw-r--r--   0        0        0    39244 2023-11-25 20:59:50.919919 pygamextras-1.1.4/main/PygameXtras/src/classes/Entity.py
--rw-r--r--   0        0        0    13596 2023-12-02 00:50:40.682100 pygamextras-1.1.4/main/PygameXtras/src/classes/Entry.py
--rw-r--r--   0        0        0    11526 2023-09-23 15:52:44.078009 pygamextras-1.1.4/main/PygameXtras/src/classes/Function.py
--rw-r--r--   0        0        0     6867 2023-11-25 20:48:13.714174 pygamextras-1.1.4/main/PygameXtras/src/classes/Functions.py
--rw-r--r--   0        0        0     5114 2023-11-25 20:49:10.824661 pygamextras-1.1.4/main/PygameXtras/src/classes/Keyboard.py
--rw-r--r--   0        0        0    34983 2023-11-25 20:59:58.646965 pygamextras-1.1.4/main/PygameXtras/src/classes/Label.py
--rw-r--r--   0        0        0     6052 2023-09-23 15:51:24.540925 pygamextras-1.1.4/main/PygameXtras/src/classes/Messagebox.py
--rw-r--r--   0        0        0      480 2023-01-08 13:28:54.080041 pygamextras-1.1.4/main/PygameXtras/src/classes/OneClickManager.py
--rw-r--r--   0        0        0    20637 2023-09-23 15:51:15.063234 pygamextras-1.1.4/main/PygameXtras/src/classes/Paragraph.py
--rw-r--r--   0        0        0     1492 2023-11-25 20:43:20.479244 pygamextras-1.1.4/main/PygameXtras/src/classes/PerformanceGraph.py
--rw-r--r--   0        0        0     5561 2023-09-23 15:51:09.818079 pygamextras-1.1.4/main/PygameXtras/src/classes/PlayStationController.py
--rw-r--r--   0        0        0     2792 2023-09-23 15:51:05.104310 pygamextras-1.1.4/main/PygameXtras/src/classes/PopupMessage.py
--rw-r--r--   0        0        0    25214 2023-09-23 15:50:41.846248 pygamextras-1.1.4/main/PygameXtras/src/classes/RandomClasses.py
--rw-r--r--   0        0        0     6651 2023-09-23 15:50:58.115828 pygamextras-1.1.4/main/PygameXtras/src/classes/ScrollableButtonList.py
--rw-r--r--   0        0        0     4480 2023-01-08 13:33:47.321223 pygamextras-1.1.4/main/PygameXtras/src/classes/Spritesheet.py
--rw-r--r--   0        0        0     2235 2023-01-08 13:34:43.904812 pygamextras-1.1.4/main/PygameXtras/src/classes/Table.py
--rw-r--r--   0        0        0        0 2023-09-23 15:31:37.487011 pygamextras-1.1.4/main/PygameXtras/src/images/__init__.py
--rw-r--r--   0        0        0      410 2022-12-18 00:36:16.366358 pygamextras-1.1.4/main/PygameXtras/src/images/decrease_size.png
--rw-r--r--   0        0        0      418 2022-12-18 00:36:15.311921 pygamextras-1.1.4/main/PygameXtras/src/images/increase_size.png
--rw-r--r--   0        0        0     1724 2023-09-23 15:53:58.435943 pygamextras-1.1.4/main/PygameXtras/test/Bar.py
--rw-r--r--   0        0        0     1445 2023-09-23 15:54:10.083261 pygamextras-1.1.4/main/PygameXtras/test/CustomTemplate.py
--rw-r--r--   0        0        0      988 2023-09-23 15:54:18.546103 pygamextras-1.1.4/main/PygameXtras/test/Entry.py
--rw-r--r--   0        0        0     1927 2023-09-23 15:54:24.219499 pygamextras-1.1.4/main/PygameXtras/test/Label.py
--rw-r--r--   0        0        0     1687 2023-09-23 15:54:56.993224 pygamextras-1.1.4/main/PygameXtras/test/PopupMessage.py
--rw-r--r--   0        0        0      483 2024-02-16 00:22:42.664226 pygamextras-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      244 2023-12-04 14:48:57.853907 pygamextras-1.1.4/README.md
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 pygamextras-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-09-24 01:46:21.865382 pygamextras-1.1.5/LICENSE.txt
+-rw-r--r--   0        0        0       28 2023-09-23 15:29:20.709795 pygamextras-1.1.5/main/PygameXtras/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-23 16:11:25.887474 pygamextras-1.1.5/main/PygameXtras/src/__init__.py
+-rw-r--r--   0        0        0      772 2024-05-09 23:08:33.613728 pygamextras-1.1.5/main/PygameXtras/src/classes/__init__.py
+-rw-r--r--   0        0        0     9617 2023-11-25 20:44:04.832441 pygamextras-1.1.5/main/PygameXtras/src/classes/Bar.py
+-rw-r--r--   0        0        0     3900 2023-09-23 15:53:12.120929 pygamextras-1.1.5/main/PygameXtras/src/classes/Button.py
+-rw-r--r--   0        0        0     5619 2024-02-16 00:25:11.507109 pygamextras-1.1.5/main/PygameXtras/src/classes/C.py
+-rw-r--r--   0        0        0     1625 2024-03-11 20:52:23.893174 pygamextras-1.1.5/main/PygameXtras/src/classes/Collisions.py
+-rw-r--r--   0        0        0    12895 2023-04-21 00:07:14.084627 pygamextras-1.1.5/main/PygameXtras/src/classes/Colors.py
+-rw-r--r--   0        0        0     2555 2023-11-25 20:46:23.639451 pygamextras-1.1.5/main/PygameXtras/src/classes/CustomTemplate.py
+-rw-r--r--   0        0        0    39244 2023-11-25 20:59:50.919919 pygamextras-1.1.5/main/PygameXtras/src/classes/Entity.py
+-rw-r--r--   0        0        0    13596 2023-12-02 00:50:40.682100 pygamextras-1.1.5/main/PygameXtras/src/classes/Entry.py
+-rw-r--r--   0        0        0    11526 2023-09-23 15:52:44.078009 pygamextras-1.1.5/main/PygameXtras/src/classes/Function.py
+-rw-r--r--   0        0        0     6867 2023-11-25 20:48:13.714174 pygamextras-1.1.5/main/PygameXtras/src/classes/Functions.py
+-rw-r--r--   0        0        0     5114 2023-11-25 20:49:10.824661 pygamextras-1.1.5/main/PygameXtras/src/classes/Keyboard.py
+-rw-r--r--   0        0        0    34983 2023-11-25 20:59:58.646965 pygamextras-1.1.5/main/PygameXtras/src/classes/Label.py
+-rw-r--r--   0        0        0     6052 2023-09-23 15:51:24.540925 pygamextras-1.1.5/main/PygameXtras/src/classes/Messagebox.py
+-rw-r--r--   0        0        0      480 2023-01-08 13:28:54.080041 pygamextras-1.1.5/main/PygameXtras/src/classes/OneClickManager.py
+-rw-r--r--   0        0        0    20637 2023-09-23 15:51:15.063234 pygamextras-1.1.5/main/PygameXtras/src/classes/Paragraph.py
+-rw-r--r--   0        0        0     1492 2023-11-25 20:43:20.479244 pygamextras-1.1.5/main/PygameXtras/src/classes/PerformanceGraph.py
+-rw-r--r--   0        0        0     5561 2023-09-23 15:51:09.818079 pygamextras-1.1.5/main/PygameXtras/src/classes/PlayStationController.py
+-rw-r--r--   0        0        0     6841 2024-05-09 23:08:05.577317 pygamextras-1.1.5/main/PygameXtras/src/classes/PlayStationVectorGraphics/psvg.py
+-rw-r--r--   0        0        0     4685 2024-05-09 23:06:43.658058 pygamextras-1.1.5/main/PygameXtras/src/classes/PlayStationVectorGraphics/psvg_util.py
+-rw-r--r--   0        0        0     2792 2023-09-23 15:51:05.104310 pygamextras-1.1.5/main/PygameXtras/src/classes/PopupMessage.py
+-rw-r--r--   0        0        0    25214 2023-09-23 15:50:41.846248 pygamextras-1.1.5/main/PygameXtras/src/classes/RandomClasses.py
+-rw-r--r--   0        0        0     6651 2023-09-23 15:50:58.115828 pygamextras-1.1.5/main/PygameXtras/src/classes/ScrollableButtonList.py
+-rw-r--r--   0        0        0     4480 2023-01-08 13:33:47.321223 pygamextras-1.1.5/main/PygameXtras/src/classes/Spritesheet.py
+-rw-r--r--   0        0        0     2235 2023-01-08 13:34:43.904812 pygamextras-1.1.5/main/PygameXtras/src/classes/Table.py
+-rw-r--r--   0        0        0        0 2023-09-23 15:31:37.487011 pygamextras-1.1.5/main/PygameXtras/src/images/__init__.py
+-rw-r--r--   0        0        0      410 2022-12-18 00:36:16.366358 pygamextras-1.1.5/main/PygameXtras/src/images/decrease_size.png
+-rw-r--r--   0        0        0      418 2022-12-18 00:36:15.311921 pygamextras-1.1.5/main/PygameXtras/src/images/increase_size.png
+-rw-r--r--   0        0        0     1724 2023-09-23 15:53:58.435943 pygamextras-1.1.5/main/PygameXtras/test/Bar.py
+-rw-r--r--   0        0        0     1445 2023-09-23 15:54:10.083261 pygamextras-1.1.5/main/PygameXtras/test/CustomTemplate.py
+-rw-r--r--   0        0        0      988 2023-09-23 15:54:18.546103 pygamextras-1.1.5/main/PygameXtras/test/Entry.py
+-rw-r--r--   0        0        0     1927 2023-09-23 15:54:24.219499 pygamextras-1.1.5/main/PygameXtras/test/Label.py
+-rw-r--r--   0        0        0     1687 2023-09-23 15:54:56.993224 pygamextras-1.1.5/main/PygameXtras/test/PopupMessage.py
+-rw-r--r--   0        0        0      483 2024-05-09 23:09:20.027354 pygamextras-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-12-04 14:48:57.853907 pygamextras-1.1.5/README.md
+-rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 pygamextras-1.1.5/PKG-INFO
```

### Comparing `pygamextras-1.1.4/LICENSE.txt` & `pygamextras-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/__init__.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from .RandomClasses import *
 from .Bar import Bar
 from .Button import Button
 from .C import C
 from .Colors import Colors
 from .CustomTemplate import CustomTemplate
 from .Entity import Entity
 from .Entry import Entry
@@ -11,11 +10,13 @@
 from .Keyboard import Keyboard
 from .Label import Label
 from .Messagebox import Messagebox
 from .OneClickManager import OneClickManager
 from .Paragraph import Paragraph
 from .PerformanceGraph import PerformanceGraph
 from .PlayStationController import PlayStationController
+from .PlayStationVectorGraphics.psvg import PSVG
 from .PopupMessage import PopupMessage
+from .RandomClasses import *
 from .ScrollableButtonList import ScrollableButtonList
 from .Spritesheet import Spritesheet
-from .Table import Table
+from .Table import Table
```

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/Bar.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/Bar.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/Button.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/Button.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/C.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/C.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/Colors.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/Colors.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/CustomTemplate.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/CustomTemplate.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/Entity.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/Entity.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/Entry.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/Entry.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/Function.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/Function.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/Functions.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/Functions.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/Keyboard.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/Keyboard.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/Label.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/Label.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/Messagebox.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/Messagebox.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/Paragraph.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/Paragraph.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/PerformanceGraph.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/PerformanceGraph.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/PlayStationController.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/PlayStationController.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/PopupMessage.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/PopupMessage.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/RandomClasses.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/RandomClasses.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/ScrollableButtonList.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/ScrollableButtonList.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/Spritesheet.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/Spritesheet.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/src/classes/Table.py` & `pygamextras-1.1.5/main/PygameXtras/src/classes/Table.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/test/Bar.py` & `pygamextras-1.1.5/main/PygameXtras/test/Bar.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/test/CustomTemplate.py` & `pygamextras-1.1.5/main/PygameXtras/test/CustomTemplate.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/test/Entry.py` & `pygamextras-1.1.5/main/PygameXtras/test/Entry.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/test/Label.py` & `pygamextras-1.1.5/main/PygameXtras/test/Label.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/main/PygameXtras/test/PopupMessage.py` & `pygamextras-1.1.5/main/PygameXtras/test/PopupMessage.py`

 * *Files identical despite different names*

### Comparing `pygamextras-1.1.4/PKG-INFO` & `pygamextras-1.1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: PygameXtras
-Version: 1.1.4
+Version: 1.1.5
 Summary: Labels, Buttons and much more for pygame
 Home-page: https://github.com/marcelm9/PygameXtras.git
 License: MIT
 Author: marcelm9
 Author-email: marcel.menzel09@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pygame-ce (>=2.4.0,<3.0.0)
 Project-URL: Repository, https://github.com/marcelm9/PygameXtras.git
 Description-Content-Type: text/markdown
 
 # PygameXtras
 PygameXtras is a library designed to make programming with pygame easier. It supplies classes that aim at reducing the time and effort that go into everyday tasks like displaying text, creating buttons, managing entry forms, etc.
```

