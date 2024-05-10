# Comparing `tmp/easy_gui_jupyter-2024.5.10.tar.gz` & `tmp/easy_gui_jupyter-2024.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_gui_jupyter-2024.5.10.tar", max compression
+gzip compressed data, was "easy_gui_jupyter-2024.5.8.tar", max compression
```

## Comparing `easy_gui_jupyter-2024.5.10.tar` & `easy_gui_jupyter-2024.5.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1104 2024-05-08 10:31:35.279760 easy_gui_jupyter-2024.5.10/LICENSE.txt
--rw-r--r--   0        0        0     2674 2024-05-08 10:29:30.553206 easy_gui_jupyter-2024.5.10/README.md
--rw-r--r--   0        0        0       52 2024-05-08 11:08:51.866358 easy_gui_jupyter-2024.5.10/easy_gui_jupyter/__init__.py
--rw-r--r--   0        0        0     9801 2024-05-10 17:33:46.474130 easy_gui_jupyter-2024.5.10/easy_gui_jupyter/easy_gui_jupyter.py
--rw-r--r--   0        0        0      840 2024-05-10 17:54:22.559440 easy_gui_jupyter-2024.5.10/pyproject.toml
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 easy_gui_jupyter-2024.5.10/PKG-INFO
+-rw-r--r--   0        0        0     1104 2024-05-08 10:31:35.279760 easy_gui_jupyter-2024.5.8/LICENSE.txt
+-rw-r--r--   0        0        0     2674 2024-05-08 10:29:30.553206 easy_gui_jupyter-2024.5.8/README.md
+-rw-r--r--   0        0        0       52 2024-05-08 11:08:51.866358 easy_gui_jupyter-2024.5.8/easy_gui_jupyter/__init__.py
+-rw-r--r--   0        0        0     9311 2024-05-08 11:08:51.867208 easy_gui_jupyter-2024.5.8/easy_gui_jupyter/easy_gui_jupyter.py
+-rw-r--r--   0        0        0      840 2024-05-08 14:12:51.366763 easy_gui_jupyter-2024.5.8/pyproject.toml
+-rw-r--r--   0        0        0     3312 1970-01-01 00:00:00.000000 easy_gui_jupyter-2024.5.8/PKG-INFO
```

### Comparing `easy_gui_jupyter-2024.5.10/LICENSE.txt` & `easy_gui_jupyter-2024.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easy_gui_jupyter-2024.5.10/README.md` & `easy_gui_jupyter-2024.5.8/README.md`

 * *Files identical despite different names*

### Comparing `easy_gui_jupyter-2024.5.10/easy_gui_jupyter/easy_gui_jupyter.py` & `easy_gui_jupyter-2024.5.8/easy_gui_jupyter/easy_gui_jupyter.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     Note:
         This class simplifies the creation of GUIs in Jupyter notebooks using ipywidgets. It provides a variety of methods for adding different types of widgets to the GUI, and it allows for saving and loading widget values to maintain user settings across sessions.
     """
 
     def __init__(self, title="basic_gui", width="50%"):
         """
         Container for widgets.
-        :param title: title of the widget container
         :param width: width of the widget container
         """
         self._layout = widgets.Layout(width=width)
         self._style = {"description_width": "initial"}
         self._widgets = {}
         self._nLabels = 0
         self._main_display = widgets.VBox()
@@ -99,29 +98,25 @@
         :param args: args for the widget
         :param kwargs: kwargs for the widget
         """
         self._widgets[tag] = widgets.Button(
             *args, **kwargs, layout=self._layout, style=self._style
         )
 
-    def add_text(self, tag, *args, remember_value=False, **kwargs):
+    def add_text(self, tag, *args, **kwargs):
         """
         Add a text widget to the container.
         :param tag: tag to identify the widget
         :param args: args for the widget
-        :param remember_value: remember the last value
         :param kwargs: kwargs for the widget
 
         Example:
             >>> gui = EasyGUI()
             >>> gui.add_text("text", value="Hello, world!")
         """
-        if remember_value and tag in self.cfg:
-            kwargs["value"] = str(self.cfg[tag])
-
         self._widgets[tag] = widgets.Text(
             *args, **kwargs, layout=self._layout, style=self._style
         )
 
     def add_int_slider(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a integer slider widget to the container.
@@ -131,15 +126,15 @@
         :param kwargs: kwargs for the widget
         """
         if (
             remember_value
             and tag in self.cfg
             and kwargs["min"] <= self.cfg[tag] <= kwargs["max"]
         ):
-            kwargs["value"] = int(self.cfg[tag])
+            kwargs["value"] = self.cfg[tag]
         self._widgets[tag] = widgets.IntSlider(
             *args, **kwargs, layout=self._layout, style=self._style
         )
 
     def add_float_slider(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a float slider widget to the container.
@@ -231,23 +226,14 @@
                 pass
             elif hasattr(self._widgets[tag], "value"):
                 self.cfg[tag] = self._widgets[tag].value
         self._cfg[self._title] = self.cfg
         with open(self._config_file, "w") as f:
             yaml.dump(self._cfg, f)
 
-    def restore_default_settings(self):
-        # restore default settings
-        self.cfg = {}
-        self._cfg[self._title] = {}
-        with open(self._config_file, "w") as f:
-            yaml.dump(self._cfg, f)
-        self.clear()
-        self.show()
-
     def show(self):
         """
         Show the widgets in the container.
         """
         # display the widgets
         self._main_display.children = tuple(self._widgets.values())
         clear_output()
```

### Comparing `easy_gui_jupyter-2024.5.10/pyproject.toml` & `easy_gui_jupyter-2024.5.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_gui_jupyter"
-version = "2024.05.10"
+version = "2024.05.08"
 description = "Simplify the creation of GUI elements in Jupyter notebooks"
 authors = [    
     "Ricardo Henriques <ricardo@henriqueslab.org>", 
     "Bruno Saraiva <bruno.msaraiva2@gmail.com>",
     "António Brito <antmsbrito95@gmail.com>"
     ]
 readme = "README.md"
```

### Comparing `easy_gui_jupyter-2024.5.10/PKG-INFO` & `easy_gui_jupyter-2024.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_gui_jupyter
-Version: 2024.5.10
+Version: 2024.5.8
 Summary: Simplify the creation of GUI elements in Jupyter notebooks
 Author: Ricardo Henriques
 Author-email: ricardo@henriqueslab.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

