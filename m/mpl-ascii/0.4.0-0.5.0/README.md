# Comparing `tmp/mpl_ascii-0.4.0.tar.gz` & `tmp/mpl_ascii-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_ascii-0.4.0.tar", last modified: Sun May  5 16:04:28 2024, max compression
+gzip compressed data, was "mpl_ascii-0.5.0.tar", last modified: Fri May 10 08:49:02 2024, max compression
```

## Comparing `mpl_ascii-0.4.0.tar` & `mpl_ascii-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,78 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-05 16:04:28.904389 mpl_ascii-0.4.0/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2024-04-25 16:42:37.000000 mpl_ascii-0.4.0/LICENSE
--rw-r--r--   0 chris     (1000) chris     (1000)     5652 2024-05-05 16:04:28.904389 mpl_ascii-0.4.0/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     5253 2024-04-30 17:38:47.000000 mpl_ascii-0.4.0/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-05 16:04:28.904389 mpl_ascii-0.4.0/mpl_ascii/
--rw-rw-r--   0 chris     (1000) chris     (1000)     3413 2024-05-04 12:09:44.000000 mpl_ascii-0.4.0/mpl_ascii/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1239 2024-04-30 16:43:02.000000 mpl_ascii-0.4.0/mpl_ascii/ascii_canvas.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2055 2024-04-30 16:45:38.000000 mpl_ascii-0.4.0/mpl_ascii/color_map.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12382 2024-05-05 15:53:15.000000 mpl_ascii-0.4.0/mpl_ascii/draw.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1342 2024-04-30 16:37:32.000000 mpl_ascii-0.4.0/mpl_ascii/overlay.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      274 2024-04-25 16:43:43.000000 mpl_ascii-0.4.0/mpl_ascii/tools.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-05 16:04:28.904389 mpl_ascii-0.4.0/mpl_ascii.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     5652 2024-05-05 16:04:28.000000 mpl_ascii-0.4.0/mpl_ascii.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      347 2024-05-05 16:04:28.000000 mpl_ascii-0.4.0/mpl_ascii.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-05-05 16:04:28.000000 mpl_ascii-0.4.0/mpl_ascii.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       31 2024-05-05 16:04:28.000000 mpl_ascii-0.4.0/mpl_ascii.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       10 2024-05-05 16:04:28.000000 mpl_ascii-0.4.0/mpl_ascii.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      513 2024-05-05 16:01:04.000000 mpl_ascii-0.4.0/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-05-05 16:04:28.904389 mpl_ascii-0.4.0/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-05 16:04:28.904389 mpl_ascii-0.4.0/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)     4510 2024-04-30 16:36:55.000000 mpl_ascii-0.4.0/tests/test_overlay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:49:01.999471 mpl_ascii-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:49:01.983471 mpl_ascii-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:49:01.987471 mpl_ascii-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-10 08:49:01.999471 mpl_ascii-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:49:01.995471 mpl_ascii-0.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_chart.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_stacked.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/barh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/barh.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/categorical_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/categorical_variables.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/cohere.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/csd_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/csd_demo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/double_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/double_plot.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/errorbars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/errorbars.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/errorbars_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/errorbars_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/errorbars_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/errorbars_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/errorbars_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/errorbars_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/hist_best_fit_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/hist_best_fit_line.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/hist_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/hist_simple.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/hist_simple_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/hist_simple_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/line_markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38794 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/line_markers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/lines_multi_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/lines_multi_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/scatter_multi_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/scatter_multi_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/simple_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/simple_plot.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:49:01.995471 mpl_ascii-0.5.0/mpl_ascii/
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/mpl_ascii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/mpl_ascii/ascii_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/mpl_ascii/color_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/mpl_ascii/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/mpl_ascii/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/mpl_ascii/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:49:01.999471 mpl_ascii-0.5.0/mpl_ascii.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-10 08:49:01.000000 mpl_ascii-0.5.0/mpl_ascii.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-10 08:49:01.000000 mpl_ascii-0.5.0/mpl_ascii.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:49:01.000000 mpl_ascii-0.5.0/mpl_ascii.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-10 08:49:01.000000 mpl_ascii-0.5.0/mpl_ascii.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 08:49:01.000000 mpl_ascii-0.5.0/mpl_ascii.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:49:01.999471 mpl_ascii-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:49:01.999471 mpl_ascii-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/tests/test_overlay.py
```

### Comparing `mpl_ascii-0.4.0/LICENSE` & `mpl_ascii-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.4.0/PKG-INFO` & `mpl_ascii-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: mpl_ascii
-Version: 0.4.0
+Version: 0.5.0
 Summary: A matplotlib backend that produces plots using only ASCII characters
+Author: Chris Cave
+Maintainer: Chris Cave
 License: MIT License
 Project-URL: Homepage, https://github.com/chriscave/mpl_ascii
 Keywords: matplotlib,plotting,ASCII
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: matplotlib>=3.8.3
+Requires-Dist: matplotlib>=3.5.3
 Requires-Dist: rich>=13.7.1
 
 # mpl_ascii
 
-A matplotlib backend that produces plots using only ASCII characters. It is available for python 3.10+.
+A matplotlib backend that produces plots using only ASCII characters. It is available for python 3.7+.
 
 ## Quick start
 
 Install `mpl_ascii` using pip
 
 ```bash
 pip install mpl_ascii
```

### Comparing `mpl_ascii-0.4.0/README.md` & `mpl_ascii-0.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # mpl_ascii
 
-A matplotlib backend that produces plots using only ASCII characters. It is available for python 3.10+.
+A matplotlib backend that produces plots using only ASCII characters. It is available for python 3.7+.
 
 ## Quick start
 
 Install `mpl_ascii` using pip
 
 ```bash
 pip install mpl_ascii
```

### Comparing `mpl_ascii-0.4.0/mpl_ascii/__init__.py` & `mpl_ascii-0.5.0/mpl_ascii/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,26 @@
+from typing import Optional
 from matplotlib._pylab_helpers import Gcf
 
 from matplotlib.backends.backend_agg import (
     FigureManagerBase,
-    RendererAgg,
     FigureCanvasAgg,
 )
 from matplotlib.figure import Figure
 
 from mpl_ascii.ascii_canvas import AsciiCanvas
-from mpl_ascii.color_map import Char, ax_color_map
+from mpl_ascii.color_map import ax_color_map
 from mpl_ascii.draw import draw_ax
 
 from rich.console import Console
 
 AXES_WIDTH = 150
 AXES_HEIGHT = 40
 ENABLE_COLORS = True
 
-class RendererAscii(RendererAgg):
-
-    def __init__(self, width, height, dpi):
-        super(RendererAscii, self).__init__(width, height, dpi)
-        self.texts = []
-        self.tick_info = []
-
-    def clear(self):
-        super(RendererAscii, self).clear()
-        self.texts = []
-        self.tick_info = []
-
-    def draw_text(self, gc, x, y, s, prop, angle, ismath=False, mtext=None):
-        super(RendererAscii, self).draw_text(
-            gc, x, y, s, prop, angle, ismath=ismath, mtext=mtext
-        )
-
-        if mtext is not None:
-            self.texts.append(mtext)
-
-
 def show():
     for manager in Gcf.get_all_fig_managers():
         canvas = manager.canvas
         canvas.draw()
         console = Console()
         if ENABLE_COLORS:
             fig = canvas.to_txt_with_color()
@@ -50,26 +29,16 @@
             fig = canvas.to_txt()
             print(fig)
 
 
 
 class FigureCanvasAscii(FigureCanvasAgg):
 
-    def __init__(self, figure: Figure | None = ...) -> None:
+    def __init__(self, figure: Optional[Figure] = ...) -> None:
         super().__init__(figure)
-        self.tick_info = []
-
-    def get_renderer(self):
-        w, h = self.figure.bbox.size
-        key = w, h, self.figure.dpi
-        reuse_renderer = self._lastKey == key
-        if not reuse_renderer:
-            self.renderer = RendererAscii(w, h, self.figure.dpi)
-            self._lastKey = key
-        return self.renderer
 
     def to_txt_with_color(self, sep="\n", tw=240, invert=False, threshold=200):
         self.draw()
 
         figure = self.figure
         axes_height = AXES_HEIGHT
         axes_width = AXES_WIDTH
```

### Comparing `mpl_ascii-0.4.0/mpl_ascii/ascii_canvas.py` & `mpl_ascii-0.5.0/mpl_ascii/ascii_canvas.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.4.0/mpl_ascii/color_map.py` & `mpl_ascii-0.5.0/mpl_ascii/color_map.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.4.0/mpl_ascii/draw.py` & `mpl_ascii-0.5.0/mpl_ascii/draw.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.4.0/mpl_ascii/overlay.py` & `mpl_ascii-0.5.0/mpl_ascii/overlay.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.4.0/mpl_ascii.egg-info/PKG-INFO` & `mpl_ascii-0.5.0/mpl_ascii.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: mpl_ascii
-Version: 0.4.0
+Version: 0.5.0
 Summary: A matplotlib backend that produces plots using only ASCII characters
+Author: Chris Cave
+Maintainer: Chris Cave
 License: MIT License
 Project-URL: Homepage, https://github.com/chriscave/mpl_ascii
 Keywords: matplotlib,plotting,ASCII
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: matplotlib>=3.8.3
+Requires-Dist: matplotlib>=3.5.3
 Requires-Dist: rich>=13.7.1
 
 # mpl_ascii
 
-A matplotlib backend that produces plots using only ASCII characters. It is available for python 3.10+.
+A matplotlib backend that produces plots using only ASCII characters. It is available for python 3.7+.
 
 ## Quick start
 
 Install `mpl_ascii` using pip
 
 ```bash
 pip install mpl_ascii
```

### Comparing `mpl_ascii-0.4.0/tests/test_overlay.py` & `mpl_ascii-0.5.0/tests/test_overlay.py`

 * *Files identical despite different names*

