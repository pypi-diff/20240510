# Comparing `tmp/junkie-rfglab-2023.9.3.tar.gz` & `tmp/junkie_rfglab-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junkie-rfglab-2023.9.3.tar", last modified: Fri Sep 22 21:53:58 2023, max compression
+gzip compressed data, was "junkie_rfglab-2024.5.0.tar", last modified: Fri May 10 18:55:26 2024, max compression
```

## Comparing `junkie-rfglab-2023.9.3.tar` & `junkie_rfglab-2024.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-09-22 21:53:58.345089 junkie-rfglab-2023.9.3/
--rw-r--r--   0 rodrigo    (501) staff       (20)    33148 2023-05-12 19:44:56.000000 junkie-rfglab-2023.9.3/LICENSE
--rw-r--r--   0 rodrigo    (501) staff       (20)     4999 2023-09-22 21:53:58.344916 junkie-rfglab-2023.9.3/PKG-INFO
--rw-r--r--   0 rodrigo    (501) staff       (20)     4267 2023-09-21 20:21:37.000000 junkie-rfglab-2023.9.3/README.md
--rw-r--r--   0 rodrigo    (501) staff       (20)    14192 2023-09-22 21:53:21.000000 junkie-rfglab-2023.9.3/junkie.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-09-22 21:53:58.344723 junkie-rfglab-2023.9.3/junkie_rfglab.egg-info/
--rw-r--r--   0 rodrigo    (501) staff       (20)     4999 2023-09-22 21:53:58.000000 junkie-rfglab-2023.9.3/junkie_rfglab.egg-info/PKG-INFO
--rw-r--r--   0 rodrigo    (501) staff       (20)      226 2023-09-22 21:53:58.000000 junkie-rfglab-2023.9.3/junkie_rfglab.egg-info/SOURCES.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)        1 2023-09-22 21:53:58.000000 junkie-rfglab-2023.9.3/junkie_rfglab.egg-info/dependency_links.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)       69 2023-09-22 21:53:58.000000 junkie-rfglab-2023.9.3/junkie_rfglab.egg-info/requires.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)        7 2023-09-22 21:53:58.000000 junkie-rfglab-2023.9.3/junkie_rfglab.egg-info/top_level.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)      840 2023-08-02 16:25:55.000000 junkie-rfglab-2023.9.3/pyproject.toml
--rw-r--r--   0 rodrigo    (501) staff       (20)       38 2023-09-22 21:53:58.345125 junkie-rfglab-2023.9.3/setup.cfg
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-05-10 18:55:26.771715 junkie_rfglab-2024.5.0/
+-rw-r--r--   0 rodrigo    (501) staff       (20)    33148 2023-05-12 19:44:56.000000 junkie_rfglab-2024.5.0/LICENSE
+-rw-r--r--   0 rodrigo    (501) staff       (20)     6202 2024-05-10 18:55:26.771581 junkie_rfglab-2024.5.0/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) staff       (20)     5470 2024-05-10 18:47:10.000000 junkie_rfglab-2024.5.0/README.md
+-rw-r--r--   0 rodrigo    (501) staff       (20)    14721 2024-05-10 18:32:32.000000 junkie_rfglab-2024.5.0/junkie.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-05-10 18:55:26.771408 junkie_rfglab-2024.5.0/junkie_rfglab.egg-info/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     6202 2024-05-10 18:55:26.000000 junkie_rfglab-2024.5.0/junkie_rfglab.egg-info/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) staff       (20)      226 2024-05-10 18:55:26.000000 junkie_rfglab-2024.5.0/junkie_rfglab.egg-info/SOURCES.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)        1 2024-05-10 18:55:26.000000 junkie_rfglab-2024.5.0/junkie_rfglab.egg-info/dependency_links.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)       69 2024-05-10 18:55:26.000000 junkie_rfglab-2024.5.0/junkie_rfglab.egg-info/requires.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)        6 2024-05-10 18:55:26.000000 junkie_rfglab-2024.5.0/junkie_rfglab.egg-info/top_level.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)      840 2023-08-02 16:25:55.000000 junkie_rfglab-2024.5.0/pyproject.toml
+-rw-r--r--   0 rodrigo    (501) staff       (20)       38 2024-05-10 18:55:26.771745 junkie_rfglab-2024.5.0/setup.cfg
```

### Comparing `junkie-rfglab-2023.9.3/LICENSE` & `junkie_rfglab-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `junkie-rfglab-2023.9.3/PKG-INFO` & `junkie_rfglab-2024.5.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junkie-rfglab
-Version: 2023.9.3
+Version: 2024.5.0
 Summary: junkie is a JUpyter NotebooK Image Explorer
 Author-email: Rodrigo Fernandez-Gonzalez <rodrigo.fernandez.gonzalez@utoronto.ca>
 Project-URL: Homepage, https://bitbucket.com/rfg_lab/junkie
 Project-URL: Bug Tracker, https://bitbucket.com/rfg_lab/junkie/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -24,65 +24,81 @@
 
 ## Installing [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/)
 
 To install [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/), type:  
 
     $ python3 -m pip install --no-cache-dir -U junkie-rfglab
 
+[JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) can also be installed with [conda/miniconda](https://docs.conda.io/projects/conda/en/stable/user-guide/install/download.html#) or [mamba](https://anaconda.org/conda-forge/mamba) (keep in mind that [mamba](https://anaconda.org/conda-forge/mamba) is much faster):  
+
+    $ mamba install -c rodrigofg junkie-rfglab
+
 We do most of the development and testing of [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) in [Jupyter Lab](https://jupyter.org/install), so we recommend using [Jupyter Lab](https://jupyter.org/install). 
 
 ### A note on the Python interpreter
 
 [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) requires that you
 have [Python 3.10 or above](https://www.python.org/downloads/) installed.
 
 ## Using [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/)
 
-[JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) uses [matplotlib](https://matplotlib.org/) and [ipywidgets](https://ipywidgets.readthedocs.io/en/stable/), so there is some boiler plate code that you need before importing [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fbitbucket.org%2Frfg_lab%2Fjunkie/HEAD?labpath=docs%2Fusing_junkie.ipynb)
 
-```python
-import matplotlib
-%matplotlib widgets
+To start, open a notebook and import [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
 
-from junkie import junkie
-```
-
-![Importing JuNkIE](./docs/import_junkie.gif)
+    from junkie import junkie
 
 There are a few ways to open an image with [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
 
 - You can open an image with some other package (e.g. scikit-image, opencv, PIL, etc.) and invoke [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) with a [numpy ndarray](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) as the parameter:
 
-![Opening an ndarray](./docs/open_ndarray.gif)
+        import skimage.io as skio
+        astack = skio.imread('cells_movie.tif')
+        myim = junkie(astack)
 
 - You can also specifiy the path to the image that you want to open:
 
-![Opening a file path](./docs/open_file.gif)
+        myim = junkie('cells_movie.tif')
 
 - Or you can indicate a folder that contains an image sequence:
 
-![Opening a folder](./docs/open_folder.gif)
+        myim = junkie('./slices')
 
 - If there are image channels split into different files, you can also specify a tuple of strings to distinguish which files in the folder belong to which channel:
 
-![Opening mutiple channels from a folder](./docs/open_folder_multichannel.gif)
+        myim = junkie('./slices', ('488', '561'))
+
+- You can use a list of numpy arrays and/or paths to concatenate sideways (i.e. display side-by-side, but all the images must have the same dimensions!!):
+
+        myim = junkie([astack, 'cells_movie.tif'])
+
+- You can combine the list input with the [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) class method *read_image* to display image channels side-by-side:
+
+        myim = junkie([*junkie.read_image('./slices', ('488', '561'))])
 
 [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) has a couple of additional parameters:
 
 - *cmap* (str) indicates the color map used to display the image. It defaults to *'gray'*. Check [here](https://matplotlib.org/stable/tutorials/colors/colormaps.html) for a list of color maps.
 
-![Color maps](./docs/colormaps.gif)
+        myim = junkie('cells_movie.tif', cmap='viridis')
 
 - *figsize* (Tuple[int, int]) specifies the image panel size. The image aspect ratio is maintained. It defaults to *(4, 4)*.
 
-![Figure size](./docs/figsize.gif)
+        myim = junkie('cells_movie.tif', figsize=(8, 8)
 
-[JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) provides access to the standard [matplotlib](https://matplotlib.org/) toolbar, and also includes a new one with additional functionality:
+[JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) provides access to the standard [matplotlib](https://matplotlib.org/) toolbar, and also includes a second toolbar with additional functionality:
 
-![Toolbar](./docs/toolbar.gif)
+|icon|function|
+|----------------------------------------|------------------------|
+|![refresh_icon](./docs/refresh_icon.png)|rotate 90&deg; clockwise
+|![refresh_icon](./docs/arrows_h_icon.png)|flip horizontally|
+|![refresh_icon](./docs/arrows_v_icon.png)|flip vertically|
+|![refresh_icon](./docs/shield_icon.png)|invert color map|
+|![refresh_icon](./docs/area_chart_icon.png)|hide/show axes|
+|![refresh_icon](./docs/fast_forward_icon.png)|continuous/discrete update|
 
 ## [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) today
 
 As we develop and improve [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/), there may be small changes to the user interface. This is how [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) looks as of today:
 
 ![JuNkIE today](./docs/junkie_today.gif)
```

### Comparing `junkie-rfglab-2023.9.3/junkie.py` & `junkie_rfglab-2024.5.0/junkie.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import os
 from typing import List, Optional, Tuple
 
 import numpy as np
 import skimage
+import IPython
+IPython.get_ipython().run_line_magic('matplotlib', 'widget')
 import IPython.display as IPyd
 import ipywidgets as ipyw
 import matplotlib.pyplot as plt
 
-__version__: str = '2023.9.3'  # this must be here for pyproject.toml to find it.
+__version__: str = '2024.5.0'  # this must be here for pyproject.toml to find it.
 
 
 # You will need this line in your jupyter notebook: %matplotlib widget
 
 class junkie:
     """ 
     junkie: a JUpyter NotebooK Image Explorer
     junkie displays and allows exploration of n-dimensional 
     images in a Jupyter notebook. 
     
     User can interactively change the channel, time point, 
     slice plane ands slice number being viewed. 
 
     Arguments:
-    volume = 2D-5D input image as a numpy array or file/folder path
+    volume = 2D-5D input image as a numpy array OR file/folder path OR a list of
+      numpy arrays and file/folder paths to concatenate sideways (i.e. display 
+      side-by-side, but all images in the list must have the same dimensions)
     channel_strs = tuple of strings to distinguish files from different channels 
       (if opening a multichannel image from a file sequence)
     cmap = default('gray'), string for the matplotlib colormap
     figsize = default(4,4), to set the size of the figure
     
     """
     
@@ -38,19 +42,30 @@
     button_style = {'font_size': '14px'}
     image_extensions: Tuple[str] = ('.tif', '.tiff', '.jpg', '.jpeg', '.gif', '.png', '.bmp')
     colormaps: List[str] = plt.colormaps()
     
     def __init__(self, volume: np.ndarray|str, channel_strs: Optional[Tuple[str]] = ('', ), cmap:str = 'gray', figsize: Tuple[int, int] =(4,4)):
         # if volume is a str, read it as an image.
         if isinstance(volume, str):
-            volume = self.read_image(volume, channel_strs)
+            volume = junkie.read_image(volume, channel_strs)
             if volume is None:
                 # throw exception instead.
                 print(f'No volume found at that path. The current path is {os.path.curdir}.')
 
+        if isinstance(volume, list):
+            volume_list: List = []
+            for avolume in volume:
+                if isinstance(avolume, str):
+                    loaded_stack = junkie.read_image(avolume, channel_strs)
+                    if loaded_stack is not None:
+                        volume_list.append(loaded_stack)
+                elif isinstance(avolume, np.ndarray):
+                    volume_list.append(avolume)
+            volume = np.concatenate(np.asarray(volume_list), axis=volume_list[0].ndim-1)
+
         plt.style.use('dark_background')
         self.volume: np.ndarray = volume
         self.slices: np.ndarray = None
 
         match self.volume.ndim:
             case 1:
                 self.volume = np.expand_dims(self.volume, axis=(0, 1, 2, 3, ))
@@ -73,15 +88,14 @@
             self.volume = self.volume.astype(np.dtype(f'uint{min_bytes*8}'))
 
         self.color = self.volume[0]
         self.slices = self.color[0]
 
         self.cmap: str = cmap
         self.figsize: Tuple[int, int] = figsize
-        plt.set_cmap(cmap)
         self.pix_val_min_max: List = [np.min(self.color), np.max(self.color)]  # stores min and max pixels values in the current channel.
 
         self.fig = plt.figure(junkie.next_figure_index, figsize=self.figsize)
         junkie.next_figure_index += 1
         self.im_axes = None
 
         self.fig.canvas.header_visible = False  # remove the figure number; handle functions in canvas could be useful to control interaction.
@@ -112,21 +126,20 @@
             self.view_plane = self._plane_selection.value
             self.image_data = np.transpose(self.slices, junkie.orientations[self.view_plane])
             
             self._Z_slider.max = self.image_data.shape[0]-1
 
             self._setupUI()            
             
-            self.im_axes = plt.imshow(self.image_data[self.curslice,:,:], vmin=self._vmin_slider.value, vmax=self._vmax_slider.value)
-
+            plt.figure(self.fig)
+            self.im_axes = plt.imshow(self.image_data[self.curslice,:,:], vmin=self._vmin_slider.value, vmax=self._vmax_slider.value, cmap=self.cmap)
+            
         # Plot slice for the given plane and slice.
         else:
-            self.im_axes.set_data(self.image_data[self.curslice, :, :])  # much faster than another imshow.
-            self.im_axes.set_clim([self._vmin_slider.value, self._vmax_slider.value])
-            self.fig.canvas.draw_idle()
+            self.im_axes.set(data=self.image_data[self.curslice, :, :], clim=[self._vmin_slider.value, self._vmax_slider.value], cmap=self.cmap)
             
 
     def create_UI(self):
         # buttons
         # icons from https://fontawesome.com/v4/icons/ or use "description='\uXXXX'" with the unicode symbol.
         self._axes_button = ipyw.ToggleButton(icon='area-chart', layout=junkie.button_layout, style=junkie.button_style, tooltip='axes on/off', value=self.axes_visible)  
         self._axes_button.observe(self._axes_button_click, 'value')
@@ -171,15 +184,15 @@
             description='maximum pixel value:', style={'description_width': 'auto'})
         self._vmax_slider.value = self.pix_val_min_max[1]
         self._vmax_slider.observe(self._vmax_slider_change, 'value')
 
         self._autocontrast_button = ipyw.Button(description='auto', layout=junkie.button_layout, style=junkie.button_style, tooltip='auto contrast')
         self._autocontrast_button.on_click(self._autocontrast_button_click)
 
-        self._colormap_dropdown = ipyw.Dropdown(options=junkie.colormaps, value=self.cmap, tooltip='color map')
+        self._colormap_dropdown = ipyw.Dropdown(options=junkie.colormaps, value=self.cmap, tooltip='colormap')
         self._colormap_dropdown.observe(self._colormap_dropdown_change, 'value')
 
         self.new_toolbar = ipyw.VBox([ipyw.HBox([ipyw.VBox([self._channel_slider, self._t_slider, self._Z_slider]), self._plane_selection, ipyw.VBox([self._vmin_slider, self._vmax_slider, ipyw.HBox([self._autocontrast_button, self._colormap_dropdown])])]), ipyw.HBox([self._rotate_button, self._fliph_button, self._flipv_button, self._invert_button, self._axes_button, self._continuousupdate_button])])
 
         IPyd.display(self.new_toolbar)
 
     # Enables/disables UI components.
@@ -267,42 +280,38 @@
 
         #self.pix_val_min_max[0], self.pix_val_min_max[1] = self._vmin_slider.value, self._vmax_slider.value  
         self.display_slice()
 
     def _colormap_dropdown_change(self, change):
         self.cmap = self._colormap_dropdown.value
 
-        plt.set_cmap(self.cmap)
         self.display_slice()
 
-    def read_image(self, file_path: str, channel_strs: Optional[Tuple[str]]=('',)) -> Optional[np.ndarray]:
+    @classmethod
+    def read_image(cls, file_path: str, channel_strs: Optional[Tuple[str]]=('',)) -> Optional[np.ndarray]:
         im: np.ndarray = None
 
         if os.path.isfile(file_path):        
             _, ext = os.path.splitext(file_path)
 
             # First try to read images within the allowed extensions.
-            if ext in junkie.image_extensions:
+            if str.lower(ext) in junkie.image_extensions:
                 im = skimage.io.imread(file_path)
             # If the extension is unknown, try to read as a tiff file.
             else:
                 try:
                     im = skimage.io.imread(file_path, plugin='tifffile')
                 except:
                     return None
         
         elif os.path.isdir(file_path):
             channels: List[np.ndarray] = [[] for _ in channel_strs]
 
             for filename in os.listdir(file_path):
-                _, ext = os.path.splitext(os.path.join(file_path, filename))
-                if ext in junkie.image_extensions:
-                    img = skimage.io.imread(os.path.join(file_path, filename))
-                else:
-                    img = None
+                img = junkie.read_image(os.path.join(file_path, filename))
 
                 if img is not None:
                     index_list = [theindex for theindex in range(len(channel_strs)) if channel_strs[theindex] in filename]
 
                     if index_list != []:
                         channels[index_list[0]].append(img)
```

### Comparing `junkie-rfglab-2023.9.3/junkie_rfglab.egg-info/PKG-INFO` & `junkie_rfglab-2024.5.0/junkie_rfglab.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junkie-rfglab
-Version: 2023.9.3
+Version: 2024.5.0
 Summary: junkie is a JUpyter NotebooK Image Explorer
 Author-email: Rodrigo Fernandez-Gonzalez <rodrigo.fernandez.gonzalez@utoronto.ca>
 Project-URL: Homepage, https://bitbucket.com/rfg_lab/junkie
 Project-URL: Bug Tracker, https://bitbucket.com/rfg_lab/junkie/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -24,65 +24,81 @@
 
 ## Installing [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/)
 
 To install [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/), type:  
 
     $ python3 -m pip install --no-cache-dir -U junkie-rfglab
 
+[JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) can also be installed with [conda/miniconda](https://docs.conda.io/projects/conda/en/stable/user-guide/install/download.html#) or [mamba](https://anaconda.org/conda-forge/mamba) (keep in mind that [mamba](https://anaconda.org/conda-forge/mamba) is much faster):  
+
+    $ mamba install -c rodrigofg junkie-rfglab
+
 We do most of the development and testing of [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) in [Jupyter Lab](https://jupyter.org/install), so we recommend using [Jupyter Lab](https://jupyter.org/install). 
 
 ### A note on the Python interpreter
 
 [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) requires that you
 have [Python 3.10 or above](https://www.python.org/downloads/) installed.
 
 ## Using [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/)
 
-[JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) uses [matplotlib](https://matplotlib.org/) and [ipywidgets](https://ipywidgets.readthedocs.io/en/stable/), so there is some boiler plate code that you need before importing [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fbitbucket.org%2Frfg_lab%2Fjunkie/HEAD?labpath=docs%2Fusing_junkie.ipynb)
 
-```python
-import matplotlib
-%matplotlib widgets
+To start, open a notebook and import [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
 
-from junkie import junkie
-```
-
-![Importing JuNkIE](./docs/import_junkie.gif)
+    from junkie import junkie
 
 There are a few ways to open an image with [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
 
 - You can open an image with some other package (e.g. scikit-image, opencv, PIL, etc.) and invoke [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) with a [numpy ndarray](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) as the parameter:
 
-![Opening an ndarray](./docs/open_ndarray.gif)
+        import skimage.io as skio
+        astack = skio.imread('cells_movie.tif')
+        myim = junkie(astack)
 
 - You can also specifiy the path to the image that you want to open:
 
-![Opening a file path](./docs/open_file.gif)
+        myim = junkie('cells_movie.tif')
 
 - Or you can indicate a folder that contains an image sequence:
 
-![Opening a folder](./docs/open_folder.gif)
+        myim = junkie('./slices')
 
 - If there are image channels split into different files, you can also specify a tuple of strings to distinguish which files in the folder belong to which channel:
 
-![Opening mutiple channels from a folder](./docs/open_folder_multichannel.gif)
+        myim = junkie('./slices', ('488', '561'))
+
+- You can use a list of numpy arrays and/or paths to concatenate sideways (i.e. display side-by-side, but all the images must have the same dimensions!!):
+
+        myim = junkie([astack, 'cells_movie.tif'])
+
+- You can combine the list input with the [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) class method *read_image* to display image channels side-by-side:
+
+        myim = junkie([*junkie.read_image('./slices', ('488', '561'))])
 
 [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) has a couple of additional parameters:
 
 - *cmap* (str) indicates the color map used to display the image. It defaults to *'gray'*. Check [here](https://matplotlib.org/stable/tutorials/colors/colormaps.html) for a list of color maps.
 
-![Color maps](./docs/colormaps.gif)
+        myim = junkie('cells_movie.tif', cmap='viridis')
 
 - *figsize* (Tuple[int, int]) specifies the image panel size. The image aspect ratio is maintained. It defaults to *(4, 4)*.
 
-![Figure size](./docs/figsize.gif)
+        myim = junkie('cells_movie.tif', figsize=(8, 8)
 
-[JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) provides access to the standard [matplotlib](https://matplotlib.org/) toolbar, and also includes a new one with additional functionality:
+[JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) provides access to the standard [matplotlib](https://matplotlib.org/) toolbar, and also includes a second toolbar with additional functionality:
 
-![Toolbar](./docs/toolbar.gif)
+|icon|function|
+|----------------------------------------|------------------------|
+|![refresh_icon](./docs/refresh_icon.png)|rotate 90&deg; clockwise
+|![refresh_icon](./docs/arrows_h_icon.png)|flip horizontally|
+|![refresh_icon](./docs/arrows_v_icon.png)|flip vertically|
+|![refresh_icon](./docs/shield_icon.png)|invert color map|
+|![refresh_icon](./docs/area_chart_icon.png)|hide/show axes|
+|![refresh_icon](./docs/fast_forward_icon.png)|continuous/discrete update|
 
 ## [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) today
 
 As we develop and improve [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/), there may be small changes to the user interface. This is how [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) looks as of today:
 
 ![JuNkIE today](./docs/junkie_today.gif)
```

### Comparing `junkie-rfglab-2023.9.3/pyproject.toml` & `junkie_rfglab-2024.5.0/pyproject.toml`

 * *Files identical despite different names*

