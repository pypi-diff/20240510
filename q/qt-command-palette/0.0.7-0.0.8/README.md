# Comparing `tmp/qt_command_palette-0.0.7.tar.gz` & `tmp/qt_command_palette-0.0.8.tar.gz`

## Comparing `qt_command_palette-0.0.7.tar` & `qt_command_palette-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,20 @@
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/codecov.yml
--rw-r--r--   0        0        0   201915 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/example.gif
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/launch.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/setup.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/qt_command_palette/__about__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/qt_command_palette/__init__.py
--rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/qt_command_palette/_api.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/qt_command_palette/_commands.py
--rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/qt_command_palette/_list.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/qt_command_palette/_storage.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/qt_command_palette/_widget.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/tests/_file_0.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/tests/_file_1.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/tests/test_register.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/tests/test_storage.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/.gitignore
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/LICENSE.txt
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/README.md
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0   201915 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/example.gif
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/launch.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/qt_command_palette/__about__.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/qt_command_palette/__init__.py
+-rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/qt_command_palette/_api.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/qt_command_palette/_commands.py
+-rw-r--r--   0        0        0     8224 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/qt_command_palette/_list.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/qt_command_palette/_storage.py
+-rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/qt_command_palette/_widget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/tests/_file_0.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/tests/_file_1.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/tests/test_register.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/tests/test_storage.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/LICENSE.txt
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/README.md
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 qt_command_palette-0.0.8/PKG-INFO
```

### Comparing `qt_command_palette-0.0.7/.pre-commit-config.yaml` & `qt_command_palette-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.7/example.gif` & `qt_command_palette-0.0.8/example.gif`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.7/launch.py` & `qt_command_palette-0.0.8/launch.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,10 +42,14 @@
 
     group_1.register(define("only if checked"), when=_checkbox.isChecked)
 
     @group_1.register("Print widget")
     def print_widget(widget: QtW.QWidget):
         print(widget)
 
+    @group_0.register("update max rows")
+    def update_max_rows():
+        palette.set_max_rows(5)
+
     palette.install(main, "Ctrl+Shift+P")
     main.show()
     sys.exit(app.exec_())
```

### Comparing `qt_command_palette-0.0.7/qt_command_palette/_api.py` & `qt_command_palette-0.0.8/qt_command_palette/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,21 @@
 class Alignment(Enum):
     """Alignment flag of the palette."""
 
     parent = "parent"  # align to the parent widget
     screen = "screen"  # align to the screen
 
 
+class _Default:
+    pass
+
+
+_default = _Default()
+
+
 class CommandPalette:
     """The command palette interface."""
 
     def __init__(
         self, name: str, *, alignment: str | Alignment = Alignment.parent
     ) -> None:
         self._commands: list[Command] = []
@@ -132,29 +139,27 @@
 
         return wrapper if func is None else wrapper(func)
 
     def add_group(self, title: str) -> CommandGroup:
         """Add a group to the command palette."""
         return CommandGroup(title, parent=self)
 
-    __default = object()
-
-    def get_widget(self, parent: Any = __default) -> QCommandPalette:
+    def get_widget(self, parent: Any = _default) -> QCommandPalette:
         """Get a command palette widget for the given parent widget."""
         from ._widget import QCommandPalette
 
         _id = id(parent)
         if (widget := self._parent_to_palette_map.get(_id)) is None:
             widget = QCommandPalette()
             widget.extend_command(self._commands)
             self._parent_to_palette_map[_id] = widget
             self._palette_to_parent_map[id(widget)] = parent
         return widget
 
-    def show_widget(self, parent: Any = __default) -> None:
+    def show_widget(self, parent: Any = _default) -> None:
         """Show command palette widget."""
         if self.alignment is Alignment.parent:
             self.get_widget(parent).show()
         else:
             self.get_widget(parent).show_center()
         return None
 
@@ -195,14 +200,20 @@
 
             def rule(cmd: Command):
                 return cmd.title + cmd.desc
 
         self._commands.sort(key=rule, reverse=reverse)
         return None
 
+    def set_max_rows(self, value: int) -> None:
+        """Set the maximum number of rows in the command palette."""
+        for p in self._palette_to_parent_map.values():
+            self.get_widget(p)._list.set_max_rows(value)
+        return None
+
 
 class CommandGroup:
     def __init__(self, title: str, parent: CommandPalette) -> None:
         self._palette_ref = weakref.ref(parent)
         self._title = title
 
     def __repr__(self) -> str:
```

### Comparing `qt_command_palette-0.0.7/qt_command_palette/_commands.py` & `qt_command_palette-0.0.8/qt_command_palette/_commands.py`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.7/qt_command_palette/_list.py` & `qt_command_palette-0.0.8/qt_command_palette/_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,14 +110,15 @@
             self.setIndexWidget(self.model().index(i), lw)
         self.pressed.connect(self._on_clicked)
 
         self._match_color = QtGui.QColor("#468cc6")
 
     @Property(QtGui.QColor)
     def matchColor(self) -> QtGui.QColor:
+        """Color used for the matched characters."""
         return self._match_color
 
     @matchColor.setter
     def matchColor(self, color: QtGui.QColor):
         self._match_color = color
 
     def _on_clicked(self, index: QtCore.QModelIndex) -> None:
@@ -209,14 +210,30 @@
             self._current_max_index = row
             for row in range(row, max_matches):
                 self.setRowHidden(row, True)
         self.update_selection()
         self.update()
         return None
 
+    def set_max_rows(self, max_rows: int) -> None:
+        if max_rows < 0:
+            raise ValueError("max_rows must be non-negative")
+        old = self.model()._max_matches
+        if max_rows == old:
+            return None
+        elif max_rows < old:
+            self.model().beginRemoveRows(QtCore.QModelIndex(), max_rows, old - 1)
+            self.model()._max_matches = max_rows
+            self.model().endRemoveRows()
+        else:
+            self.model().beginInsertRows(QtCore.QModelIndex(), old, max_rows - 1)
+            self.model()._max_matches = max_rows
+            self.model().endInsertRows()
+        return None
+
     if TYPE_CHECKING:
 
         def model(self) -> QCommandMatchModel:
             ...
 
         def indexWidget(self, index: QtCore.QModelIndex) -> QCommandLabel:
             ...
```

### Comparing `qt_command_palette-0.0.7/qt_command_palette/_storage.py` & `qt_command_palette-0.0.8/qt_command_palette/_storage.py`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.7/qt_command_palette/_widget.py` & `qt_command_palette-0.0.8/qt_command_palette/_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def commandPalette(self) -> QCommandPalette:
         """The parent command palette widget."""
         return self.parent()
 
     def event(self, e: QtCore.QEvent):
         if e.type() != QtCore.QEvent.Type.KeyPress:
             return super().event(e)
-        e = QtGui.QKeyEvent(e)
+        assert isinstance(e, QtGui.QKeyEvent)
         if e.modifiers() in (
             Qt.KeyboardModifier.NoModifier,
             Qt.KeyboardModifier.KeypadModifier,
         ):
             key = e.key()
             if key == Qt.Key.Key_Escape:
                 self.commandPalette().hide()
```

### Comparing `qt_command_palette-0.0.7/tests/test_register.py` & `qt_command_palette-0.0.8/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.7/tests/test_storage.py` & `qt_command_palette-0.0.8/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.7/.gitignore` & `qt_command_palette-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.7/LICENSE.txt` & `qt_command_palette-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.7/README.md` & `qt_command_palette-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.7/pyproject.toml` & `qt_command_palette-0.0.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ["qtpy>=2.0.0"]
 dynamic = ["version"]
 
 [project.urls]
@@ -39,15 +40,15 @@
   "pytest-cov",
 ]
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=qt_command_palette --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
-python = ["38", "39", "310", "311"]
+python = ["38", "39", "310", "311", "312"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
   "qt_command_palette/__about__.py",
 ]
```

### Comparing `qt_command_palette-0.0.7/PKG-INFO` & `qt_command_palette-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qt-command-palette
-Version: 0.0.7
+Version: 0.0.8
 Summary: A command palette widget for Qt applications
 Project-URL: Documentation, https://github.com/unknown/qt-command-palette#readme
 Project-URL: Issues, https://github.com/unknown/qt-command-palette/issues
 Project-URL: Source, https://github.com/unknown/qt-command-palette
 Author-email: Hanjin Liu <hanjin.liu@bs.s.u-tokyo.ac.jp>
 License: MIT License
         
@@ -18,14 +18,15 @@
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: qtpy>=2.0.0
 Description-Content-Type: text/markdown
 
 # qt-command-palette
```

