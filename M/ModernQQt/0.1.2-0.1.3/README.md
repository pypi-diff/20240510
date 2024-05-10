# Comparing `tmp/modernqqt-0.1.2.tar.gz` & `tmp/modernqqt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modernqqt-0.1.2.tar", max compression
+gzip compressed data, was "modernqqt-0.1.3.tar", max compression
```

## Comparing `modernqqt-0.1.2.tar` & `modernqqt-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,32 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 modernqqt-0.1.2/LICENSE
--rw-r--r--   0        0        0      924 2024-05-10 15:57:38.790500 modernqqt-0.1.2/README.md
--rw-r--r--   0        0        0      320 2024-05-10 15:43:30.031280 modernqqt-0.1.2/modernqqt/__init__.py
--rw-r--r--   0        0        0       79 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/src/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/src/core/dialog.py
--rw-r--r--   0        0        0      101 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/src/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/src/core/font.py
--rw-r--r--   0        0        0      324 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/src/core/load.py
--rw-r--r--   0        0        0     5387 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/src/ui/angle-down.png
--rw-r--r--   0        0        0      336 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/src/ui/angle-down.svg
--rw-r--r--   0        0        0      238 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/__init__.py
--rw-r--r--   0        0        0     1317 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/button.py
--rw-r--r--   0        0        0      960 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/groups.py
--rw-r--r--   0        0        0      993 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/label.py
--rw-r--r--   0        0        0      278 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      501 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0      262 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      513 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0      286 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0      134 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0      265 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0      313 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0    10088 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/switchers.py
--rw-r--r--   0        0        0     1578 2024-05-10 14:59:21.961513 modernqqt-0.1.2/modernqqt/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0      602 2024-05-10 15:58:58.953623 modernqqt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 modernqqt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 modernqqt-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1296 2024-05-10 17:14:41.467165 modernqqt-0.1.3/README.md
+-rw-r--r--   0        0        0      320 2024-05-10 15:43:30.031280 modernqqt-0.1.3/modernqqt/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-10 16:49:32.417643 modernqqt-0.1.3/modernqqt/constructor/__init__.py
+-rw-r--r--   0        0        0      552 2024-05-10 17:10:15.186165 modernqqt-0.1.3/modernqqt/constructor/initialize.py
+-rw-r--r--   0        0        0      120 2024-05-10 17:10:15.186165 modernqqt-0.1.3/modernqqt/src/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-10 14:59:21.961513 modernqqt-0.1.3/modernqqt/src/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-10 17:10:15.186165 modernqqt-0.1.3/modernqqt/src/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-10 14:59:21.961513 modernqqt-0.1.3/modernqqt/src/core/font.py
+-rw-r--r--   0        0        0      324 2024-05-10 14:59:21.961513 modernqqt-0.1.3/modernqqt/src/core/load.py
+-rw-r--r--   0        0        0      589 2024-05-10 17:10:15.186165 modernqqt-0.1.3/modernqqt/src/core/stylesheet.py
+-rw-r--r--   0        0        0     5387 2024-05-10 14:59:21.961513 modernqqt-0.1.3/modernqqt/src/ui/angle-down.png
+-rw-r--r--   0        0        0      336 2024-05-10 14:59:21.961513 modernqqt-0.1.3/modernqqt/src/ui/angle-down.svg
+-rw-r--r--   0        0        0      238 2024-05-10 14:59:21.961513 modernqqt-0.1.3/modernqqt/widgets/__init__.py
+-rw-r--r--   0        0        0     1167 2024-05-10 17:10:15.186165 modernqqt-0.1.3/modernqqt/widgets/basic/button.py
+-rw-r--r--   0        0        0      809 2024-05-10 17:10:15.186165 modernqqt-0.1.3/modernqqt/widgets/basic/groups.py
+-rw-r--r--   0        0        0      993 2024-05-10 14:59:21.961513 modernqqt-0.1.3/modernqqt/widgets/basic/label.py
+-rw-r--r--   0        0        0      278 2024-05-10 14:59:21.961513 modernqqt-0.1.3/modernqqt/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      501 2024-05-10 14:59:21.961513 modernqqt-0.1.3/modernqqt/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0      262 2024-05-10 14:59:21.961513 modernqqt-0.1.3/modernqqt/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      513 2024-05-10 14:59:21.961513 modernqqt-0.1.3/modernqqt/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0      286 2024-05-10 14:59:21.961513 modernqqt-0.1.3/modernqqt/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0      134 2024-05-10 14:59:21.961513 modernqqt-0.1.3/modernqqt/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0      265 2024-05-10 14:59:21.961513 modernqqt-0.1.3/modernqqt/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0      313 2024-05-10 14:59:21.961513 modernqqt-0.1.3/modernqqt/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0     8915 2024-05-10 17:10:15.186165 modernqqt-0.1.3/modernqqt/widgets/basic/switchers.py
+-rw-r--r--   0        0        0     1578 2024-05-10 14:59:21.961513 modernqqt-0.1.3/modernqqt/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0       36 2024-05-10 16:49:32.417643 modernqqt-0.1.3/modernqqt/windows/__init__.py
+-rw-r--r--   0        0        0     1139 2024-05-10 17:10:15.186165 modernqqt-0.1.3/modernqqt/windows/main_window.py
+-rw-r--r--   0        0        0       58 2024-05-10 17:10:15.186165 modernqqt-0.1.3/modernqqt/windows/styles/main_window.css
+-rw-r--r--   0        0        0      602 2024-05-10 17:14:55.209864 modernqqt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2031 1970-01-01 00:00:00.000000 modernqqt-0.1.3/PKG-INFO
```

### Comparing `modernqqt-0.1.2/LICENSE` & `modernqqt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.2/modernqqt/src/core/dialog.py` & `modernqqt-0.1.3/modernqqt/src/core/dialog.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.2/modernqqt/src/core/font.py` & `modernqqt-0.1.3/modernqqt/src/core/font.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.2/modernqqt/src/ui/angle-down.png` & `modernqqt-0.1.3/modernqqt/src/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.2/modernqqt/widgets/basic/button.py` & `modernqqt-0.1.3/modernqqt/widgets/basic/button.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PySide6.QtWidgets import QPushButton
 from PySide6.QtCore import QSize
 
-from modernqqt.src.core import Loader
+from modernqqt.src.core import Loader, StyleSheetLoader
 
 from typing import Optional, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from PySide6.QtWidgets import QWidget
     from PySide6.QtGui import QFont
 
@@ -22,23 +22,19 @@
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None, 
     ) -> None:
         super().__init__(parent)
 
         if font is not None: self.setFont(font)
 
-        stylesheet_path = os.path.join(os.path.dirname(__file__), "styles/button.css")
-
-        if stylesheet is not None:
-            self.setStyleSheet(
-                Loader.load_file(stylesheet_path) + "\n" 
-                + stylesheet.replace("PushButton", "QPushButton#button")
-            )
-        else:
-            self.setStyleSheet(Loader.load_file(stylesheet_path))
+        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+            __file__, "styles/button.css", 
+            name="PushButton", obj_name="QPushButton#button",
+            stylesheet=stylesheet
+        ))
         
         self.setObjectName("button")
         self.setMinimumSize(QSize(*size))
 
         if text is not None:
             self.setText(text)
```

### Comparing `modernqqt-0.1.2/modernqqt/widgets/basic/label.py` & `modernqqt-0.1.3/modernqqt/widgets/basic/label.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.2/modernqqt/widgets/basic/styles/drop_down_menu.css` & `modernqqt-0.1.3/modernqqt/widgets/basic/styles/drop_down_menu.css`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.2/modernqqt/widgets/basic/switchers.py` & `modernqqt-0.1.3/modernqqt/widgets/basic/switchers.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     QSplitter, QComboBox, QSpinBox, 
     QLineEdit, QWidget, QHBoxLayout, 
     QSpacerItem, QSizePolicy, QCheckBox,
     QRadioButton
 )
 from PySide6.QtCore import Qt, QSize
 
-from modernqqt.src.core import Loader, FileDialog, Font
+from modernqqt.src.core import Loader, FileDialog, StyleSheetLoader
 from .button import PushButton
 
 from typing import Optional, TYPE_CHECKING
 if TYPE_CHECKING:
     from PySide6.QtGui import QFont
 
 
@@ -33,24 +33,19 @@
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         if __orientation == "horizontal": super().__init__(Qt.Orientation.Horizontal, parent)
         elif __orientation == "vertical": super().__init__(Qt.Orientation.Vertical, parent)
 
         self.setObjectName("splitter")
-
-        stylesheet_path = os.path.join(os.path.dirname(__file__), "styles/splitter.css")
-
-        if stylesheet is not None:
-            self.setStyleSheet(
-                Loader.load_file(stylesheet_path) + "\n" 
-                + stylesheet.replace("Splitter", "QSplitter#splitter")
-            )
-        else:
-            self.setStyleSheet(Loader.load_file(stylesheet_path))
+        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+            __file__, "styles/splitter.css", 
+            name="Splitter", obj_name="QSplitter#splitter",
+            stylesheet=stylesheet
+        ))
 
     def addWidget(self, widget):
         super().addWidget(widget)
         self.setCollapsible(self.indexOf(widget), False)
 
 
 class DropDownMenu(QComboBox):
@@ -78,23 +73,19 @@
         self.__values = []
 
         if values is not None: self.__values = [*values]
         self.addItems(self.__values)
         self.setObjectName("drop-down-menu")
         if font is not None: self.setFont(font)
 
-        stylesheet_path = os.path.join(os.path.dirname(__file__), "styles/drop_down_menu.css")
-
-        if stylesheet is not None:
-            self.setStyleSheet(
-                Loader.load_file(stylesheet_path) + "\n" 
-                + stylesheet.replace("DropDownMenu", "QComboBox#drop-down-menu")
-            )
-        else:
-            self.setStyleSheet(Loader.load_file(stylesheet_path))
+        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+            __file__, "styles/drop_down_menu.css", 
+            name="DropDownMenu", obj_name="QComboBox#drop-down-menu",
+            stylesheet=stylesheet
+        ))
 
     def set_items(self, *__values: str) -> None:
         self.__values = [*__values]
         self.addItems(self.__values)
 
 
 class Entry(QLineEdit):
@@ -121,23 +112,19 @@
         if placeholder is not None: self.setPlaceholderText(placeholder)
         if font is not None: self.setFont(font)
 
         self.setFixedSize(QSize(*size))
         self.setObjectName("entry")
         self.setFocusPolicy(Qt.FocusPolicy.WheelFocus)
 
-        stylesheet_path = os.path.join(os.path.dirname(__file__), "styles/entry.css")
-
-        if stylesheet is not None:
-            self.setStyleSheet(
-                Loader.load_file(stylesheet_path) + "\n" 
-                + stylesheet.replace("Entry", "QLineEdit#entry")
-            )
-        else:
-            self.setStyleSheet(Loader.load_file(stylesheet_path))
+        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+            __file__, "styles/entry.css", 
+            name="Entry", obj_name="QLineEdit#entry",
+            stylesheet=stylesheet
+        ))
 
 
 class DigitalEntry(QSpinBox):
     """
     Custom QSpinBox widget for entering digital values.
 
     Methods:
@@ -159,23 +146,19 @@
         self.setFixedSize(QSize(*size))
         if not include_buttons: self.setButtonSymbols(QSpinBox.ButtonSymbols.NoButtons)
         if font is not None: self.setFont(font)
 
         self.setObjectName("digital-entry")
         self.setRange(*range)
 
-        stylesheet_path = os.path.join(os.path.dirname(__file__), "styles/digital_entry.css")
-
-        if stylesheet is not None:
-            self.setStyleSheet(
-                Loader.load_file(stylesheet_path) + "\n" 
-                + stylesheet.replace("DigitalEntry", "QSpinBox#digital-entry")
-            )
-        else:
-            self.setStyleSheet(Loader.load_file(stylesheet_path))
+        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+            __file__, "styles/digital_entry.css", 
+            name="DigitalEntry", obj_name="QSpinBox#digital-entry",
+            stylesheet=stylesheet
+        ))
 
 
 class CheckBox(QCheckBox):
     def __init__(
             self,
             text: Optional[str] = None,
             size: tuple[int, int] = (150, 30),
@@ -193,23 +176,19 @@
         self.setCheckable(is_checkable)
         self.setDisabled(is_disabled)
 
         self.setObjectName("check-box")
         if text is not None:
             self.setText(text)
         
-        stylesheet_path = os.path.join(os.path.dirname(__file__), "styles/check_box.css")
-
-        if stylesheet is not None:
-            self.setStyleSheet(
-                Loader.load_file(stylesheet_path) + "\n" 
-                + stylesheet.replace("CheckBox", "CheckBox#check-box")
-            )
-        else:
-            self.setStyleSheet(Loader.load_file(stylesheet_path))
+        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+            __file__, "styles/check_box.css", 
+            name="CheckBox", obj_name="CheckBox#check-box",
+            stylesheet=stylesheet
+        ))
 
 
 class PathEntry(QWidget):
     """
     Custom QLineEdit widget for entering path to file and directories.
 
     Methods:
@@ -231,24 +210,20 @@
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         super().__init__(parent)
 
         self.setObjectName("path-entry")
         if font is not None: self.setFont(font)
-        
-        stylesheet_path = os.path.join(os.path.dirname(__file__), "styles/path_entry.css")
 
-        if stylesheet is not None:
-            self.setStyleSheet(
-                Loader.load_file(stylesheet_path) + "\n" 
-                + stylesheet.replace("PathEntry", "QLineEdit#path-entry")
-            )
-        else:
-            self.setStyleSheet(Loader.load_file(stylesheet_path))
+        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+            __file__, "styles/path_entry.css", 
+            name="PathEntry", obj_name="QLineEdit#path-entry",
+            stylesheet=stylesheet
+        ))
 
         self.mainLayout = QHBoxLayout()
 
         self.pathEntry = Entry(placed, placeholder, size)
 
         self.specifyPathBtn = PushButton("...")
         self.specifyPathBtn.clicked.connect(lambda: self.set_path(FileDialog.get_open_file_name()))
@@ -282,16 +257,12 @@
     ) -> None:
         super().__init__(parent)
 
         if text is not None: self.setText(text)
         self.setFixedSize(QSize(*size))
 
         self.setObjectName("radio-button")
-        stylesheet_path = os.path.join(os.path.dirname(__file__), "styles/radio_button.css")
-
-        if stylesheet is not None:
-            self.setStyleSheet(
-                Loader.load_file(stylesheet_path) + "\n" 
-                + stylesheet.replace("RadioButton", "QRadioButton#radio-button")
-            )
-        else:
-            self.setStyleSheet(Loader.load_file(stylesheet_path))
+        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+            __file__, "styles/radio_button.css", 
+            name="RadioButton", obj_name="QRadioButton#radio-button",
+            stylesheet=stylesheet
+        ))
```

### Comparing `modernqqt-0.1.2/modernqqt/widgets/basic/widgets_list.py` & `modernqqt-0.1.3/modernqqt/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `modernqqt-0.1.2/pyproject.toml` & `modernqqt-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ModernQQt"
-version = "0.1.2"
+version = "0.1.3"
 description = "ModernQt: A Cutting-Edge GUI Library Built on PyQt6 ModernQt is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now ModernQt is in development."
 authors = ["chebupelka8 <stpzamyatin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `modernqqt-0.1.2/PKG-INFO` & `modernqqt-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ModernQQt
-Version: 0.1.2
+Version: 0.1.3
 Summary: ModernQt: A Cutting-Edge GUI Library Built on PyQt6 ModernQt is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now ModernQt is in development.
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -33,14 +33,35 @@
 <h3>How to use</h3>
 
 ```sh
 pip install ModernQQt
 ```
 
 ```python
-from modernqqt.widgets import PushButton
+from modernqqt.constructor import Initialization
+from modernqqt.widgets import ...
 ...
 ```
 
-<h3>Example</h3>
-<img src="example.png">
+<h3>Examples</h3>
+<h4>Basic screen</h4>
+
+```python
+from modernqqt.constructor import Initialization
+from modernqqt.windows import MainWindow
+
+import sys
+
+
+Initialization.init(sys.argv)
+
+
+if __name__ == "__main__":
+    window = MainWindow(title="Hello", size=(600, 400))
+    window.run()
+
+    Initialization.exec()
+
+```
+
+<img src="examples/basic_screen/basic_screen.png">
```

