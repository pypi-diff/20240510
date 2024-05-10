# Comparing `tmp/waypaper-2.1.tar.gz` & `tmp/waypaper-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waypaper-2.1.tar", last modified: Thu Jan  4 12:36:02 2024, max compression
+gzip compressed data, was "waypaper-2.1.1.tar", last modified: Fri May 10 07:21:26 2024, max compression
```

## Comparing `waypaper-2.1.tar` & `waypaper-2.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2024-01-04 12:36:02.083332 waypaper-2.1/
--rw-r--r--   0 r         (1000) r         (1000)    35149 2023-12-11 19:02:06.000000 waypaper-2.1/LICENSE
--rw-r--r--   0 r         (1000) r         (1000)     4018 2024-01-04 12:36:02.083332 waypaper-2.1/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)     3128 2024-01-04 12:05:04.000000 waypaper-2.1/README.md
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2024-01-04 12:36:02.079999 waypaper-2.1/data/
--rw-r--r--   0 r         (1000) r         (1000)     1137 2024-01-01 19:30:51.000000 waypaper-2.1/data/waypaper.1.gz
--rw-r--r--   0 r         (1000) r         (1000)      227 2023-12-11 19:02:06.000000 waypaper-2.1/data/waypaper.desktop
--rw-r--r--   0 r         (1000) r         (1000)     4453 2024-01-04 09:57:32.000000 waypaper-2.1/data/waypaper.svg
--rw-r--r--   0 r         (1000) r         (1000)       91 2023-12-30 15:56:41.000000 waypaper-2.1/pyproject.toml
--rw-r--r--   0 r         (1000) r         (1000)       38 2024-01-04 12:36:02.083332 waypaper-2.1/setup.cfg
--rw-r--r--   0 r         (1000) r         (1000)     1587 2024-01-03 10:24:44.000000 waypaper-2.1/setup.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2024-01-04 12:36:02.079999 waypaper-2.1/waypaper/
--rw-r--r--   0 r         (1000) r         (1000)     2081 2024-01-04 09:22:30.000000 waypaper-2.1/waypaper/__main__.py
--rw-r--r--   0 r         (1000) r         (1000)      742 2023-12-31 16:27:53.000000 waypaper-2.1/waypaper/aboutdata.py
--rw-r--r--   0 r         (1000) r         (1000)    20951 2024-01-04 11:20:26.000000 waypaper-2.1/waypaper/app.py
--rw-r--r--   0 r         (1000) r         (1000)     3711 2024-01-04 09:17:15.000000 waypaper-2.1/waypaper/changer.py
--rw-r--r--   0 r         (1000) r         (1000)     1831 2024-01-04 09:22:27.000000 waypaper-2.1/waypaper/common.py
--rw-r--r--   0 r         (1000) r         (1000)     6666 2024-01-04 09:17:14.000000 waypaper-2.1/waypaper/config.py
--rw-r--r--   0 r         (1000) r         (1000)      861 2024-01-04 09:15:12.000000 waypaper-2.1/waypaper/options.py
--rw-r--r--   0 r         (1000) r         (1000)    17471 2023-12-30 16:57:43.000000 waypaper-2.1/waypaper/translations.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2024-01-04 12:36:02.083332 waypaper-2.1/waypaper.egg-info/
--rw-r--r--   0 r         (1000) r         (1000)     4018 2024-01-04 12:36:02.000000 waypaper-2.1/waypaper.egg-info/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)      456 2024-01-04 12:36:02.000000 waypaper-2.1/waypaper.egg-info/SOURCES.txt
--rw-r--r--   0 r         (1000) r         (1000)        1 2024-01-04 12:36:02.000000 waypaper-2.1/waypaper.egg-info/dependency_links.txt
--rw-r--r--   0 r         (1000) r         (1000)       47 2024-01-04 12:36:02.000000 waypaper-2.1/waypaper.egg-info/entry_points.txt
--rw-r--r--   0 r         (1000) r         (1000)       49 2024-01-04 12:36:02.000000 waypaper-2.1/waypaper.egg-info/requires.txt
--rw-r--r--   0 r         (1000) r         (1000)        9 2024-01-04 12:36:02.000000 waypaper-2.1/waypaper.egg-info/top_level.txt
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2024-05-10 07:21:26.718412 waypaper-2.1.1/
+-rw-r--r--   0 r         (1000) r         (1000)    35149 2024-05-10 07:19:53.000000 waypaper-2.1.1/LICENSE
+-rw-r--r--   0 r         (1000) r         (1000)     4250 2024-05-10 07:21:26.718412 waypaper-2.1.1/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)     3358 2024-05-10 07:19:53.000000 waypaper-2.1.1/README.md
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2024-05-10 07:21:26.715078 waypaper-2.1.1/data/
+-rw-r--r--   0 r         (1000) r         (1000)     1137 2024-05-10 07:19:53.000000 waypaper-2.1.1/data/waypaper.1.gz
+-rw-r--r--   0 r         (1000) r         (1000)      227 2024-05-10 07:19:53.000000 waypaper-2.1.1/data/waypaper.desktop
+-rw-r--r--   0 r         (1000) r         (1000)     4453 2024-05-10 07:19:53.000000 waypaper-2.1.1/data/waypaper.svg
+-rw-r--r--   0 r         (1000) r         (1000)       91 2024-05-10 07:19:53.000000 waypaper-2.1.1/pyproject.toml
+-rw-r--r--   0 r         (1000) r         (1000)       38 2024-05-10 07:21:26.718412 waypaper-2.1.1/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1000)     1589 2024-05-10 07:21:14.000000 waypaper-2.1.1/setup.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2024-05-10 07:21:26.718412 waypaper-2.1.1/waypaper/
+-rw-r--r--   0 r         (1000) r         (1000)     2181 2024-05-10 07:20:42.000000 waypaper-2.1.1/waypaper/__main__.py
+-rw-r--r--   0 r         (1000) r         (1000)      742 2024-05-10 07:19:53.000000 waypaper-2.1.1/waypaper/aboutdata.py
+-rw-r--r--   0 r         (1000) r         (1000)    21264 2024-05-10 07:19:53.000000 waypaper-2.1.1/waypaper/app.py
+-rw-r--r--   0 r         (1000) r         (1000)     3705 2024-05-10 07:19:53.000000 waypaper-2.1.1/waypaper/changer.py
+-rw-r--r--   0 r         (1000) r         (1000)     2005 2024-05-10 07:19:53.000000 waypaper-2.1.1/waypaper/common.py
+-rw-r--r--   0 r         (1000) r         (1000)     6876 2024-05-10 07:19:53.000000 waypaper-2.1.1/waypaper/config.py
+-rw-r--r--   0 r         (1000) r         (1000)      861 2024-05-10 07:19:53.000000 waypaper-2.1.1/waypaper/options.py
+-rw-r--r--   0 r         (1000) r         (1000)    17704 2024-05-10 07:19:53.000000 waypaper-2.1.1/waypaper/translations.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2024-05-10 07:21:26.718412 waypaper-2.1.1/waypaper.egg-info/
+-rw-r--r--   0 r         (1000) r         (1000)     4250 2024-05-10 07:21:26.000000 waypaper-2.1.1/waypaper.egg-info/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)      456 2024-05-10 07:21:26.000000 waypaper-2.1.1/waypaper.egg-info/SOURCES.txt
+-rw-r--r--   0 r         (1000) r         (1000)        1 2024-05-10 07:21:26.000000 waypaper-2.1.1/waypaper.egg-info/dependency_links.txt
+-rw-r--r--   0 r         (1000) r         (1000)       47 2024-05-10 07:21:26.000000 waypaper-2.1.1/waypaper.egg-info/entry_points.txt
+-rw-r--r--   0 r         (1000) r         (1000)       49 2024-05-10 07:21:26.000000 waypaper-2.1.1/waypaper.egg-info/requires.txt
+-rw-r--r--   0 r         (1000) r         (1000)        9 2024-05-10 07:21:26.000000 waypaper-2.1.1/waypaper.egg-info/top_level.txt
```

### Comparing `waypaper-2.1/LICENSE` & `waypaper-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `waypaper-2.1/PKG-INFO` & `waypaper-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waypaper
-Version: 2.1
+Version: 2.1.1
 Summary: GUI wallpaper setter for Wayland
 Home-page: https://github.com/anufrievroman/waypaper
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -63,14 +63,18 @@
 
 The [waypaper-git](https://aur.archlinux.org/packages/waypaper-git) package is available in AUR, thanks to *metak*. Please upvote to support the project.
 
 #### On NixOS
 
 The `waypaper` package is available thanks to Basil Keeler.
 
+#### On OpenSUSE
+
+Users of OpenSUSE [reported issue with installation](https://github.com/anufrievroman/waypaper/issues/30) via `pipx install waypaper`. This might be resolved by installing the `python311-pycairo-devel` package.
+
 ### Dependencies
 
 - `swww` or `swaybg` or `feh` or `wallutils`
 - gobject python library (it might be called `python-gobject` or `python3-gi` or `python3-gobject` in your package manager.)
 - `python-importlib_metadata`
 - `python-platformdirs`
```

### Comparing `waypaper-2.1/README.md` & `waypaper-2.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,18 @@
 
 The [waypaper-git](https://aur.archlinux.org/packages/waypaper-git) package is available in AUR, thanks to *metak*. Please upvote to support the project.
 
 #### On NixOS
 
 The `waypaper` package is available thanks to Basil Keeler.
 
+#### On OpenSUSE
+
+Users of OpenSUSE [reported issue with installation](https://github.com/anufrievroman/waypaper/issues/30) via `pipx install waypaper`. This might be resolved by installing the `python311-pycairo-devel` package.
+
 ### Dependencies
 
 - `swww` or `swaybg` or `feh` or `wallutils`
 - gobject python library (it might be called `python-gobject` or `python3-gi` or `python3-gobject` in your package manager.)
 - `python-importlib_metadata`
 - `python-platformdirs`
```

### Comparing `waypaper-2.1/data/waypaper.1.gz` & `waypaper-2.1.1/data/waypaper.1.gz`

 * *Files identical despite different names*

### Comparing `waypaper-2.1/data/waypaper.svg` & `waypaper-2.1.1/data/waypaper.svg`

 * *Files identical despite different names*

### Comparing `waypaper-2.1/setup.py` & `waypaper-2.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     license='GPL',
     entry_points={
         "gui_scripts": [
             "waypaper = waypaper.__main__:run"
         ]
     },
     install_requires=["PyGObject", "importlib_metadata", "platformdirs", "Pillow"],
-    version='2.1',
+    version='2.1.1',
     python_requires='>3.9',
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Environment :: Console",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

### Comparing `waypaper-2.1/waypaper/__main__.py` & `waypaper-2.1.1/waypaper/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Main module that runs the program and either runs GUI or just changer wallpaper"""
 
-import time
 import argparse
+import sys
+import time
 
-
-from waypaper.config import Config
+from waypaper.aboutdata import AboutData
 from waypaper.app import App
 from waypaper.changer import change_wallpaper
 from waypaper.common import get_random_file
-from waypaper.aboutdata import AboutData
-from waypaper.options import FILL_OPTIONS, BACKEND_OPTIONS
-from waypaper.translations import English, German, French, Russian, Polish, Chinese
+from waypaper.config import Config
+from waypaper.options import BACKEND_OPTIONS, FILL_OPTIONS
+from waypaper.translations import Chinese, English, French, German, Polish, Russian
 
 about = AboutData()
 cf = Config()
 
 if cf.lang == "de":
     txt = German()
 elif cf.lang == "fr":
@@ -25,46 +25,50 @@
     txt = Polish()
 elif cf.lang == "zh":
     txt = Chinese()
 else:
     txt = English()
 
 
-parser = argparse.ArgumentParser(prog = about.applicationName(), description = txt.msg_desc,
-                                 epilog = txt.msg_info)
+parser = argparse.ArgumentParser(
+    prog=about.applicationName(), description=txt.msg_desc, epilog=txt.msg_info
+)
 parser.add_argument("-v", "--version", help=txt.msg_arg_help, action="store_true")
 parser.add_argument("--restore", help=txt.msg_arg_rest, action="store_true")
 parser.add_argument("--random", help=txt.msg_arg_rand, action="store_true")
-parser.add_argument("--fill", help=txt.msg_arg_fill, action="store_true")
+parser.add_argument("--fill", help=txt.msg_arg_fill, choices=FILL_OPTIONS)
 parser.add_argument("--backend", help=txt.msg_arg_back, choices=BACKEND_OPTIONS)
 args = parser.parse_args()
 
 
 def run():
     """Read user arguments and either run GUI app or just reset the wallpaper"""
 
     cf.read_parameters_from_user_arguments(args)
 
     # Set the wallpaper and quit:
-    if args.restore:
-        for wallpaper, monitor in zip(cf.wallpaper, cf.monitors):
+    if args.restore or args.random:
+        for wallpaper, monitor in zip(cf.wallpapers, cf.monitors):
 
             if args.random:
-                wallpaper = get_random_file(cf.backend, cf.image_folder, cf.include_subfolders)
+                wallpaper = get_random_file(cf.backend, cf.image_folder, cf.include_subfolders, cf.show_hidden)
+                cf.selected_wallpaper = str(wallpaper)
+                cf.save()
 
             if wallpaper is None:
                 continue
+
             change_wallpaper(wallpaper, cf, monitor, txt)
             time.sleep(0.1)
-        exit(0)
+        sys.exit(0)
 
     # Print the version and quit:
     if args.version:
         print(f"{about.applicationName()} v.{about.applicationVersion()}")
-        exit(0)
+        sys.exit(0)
 
     # Start GUI:
     app = App(txt)
     app.run()
 
 
 if __name__ == "__main__":
```

### Comparing `waypaper-2.1/waypaper/aboutdata.py` & `waypaper-2.1.1/waypaper/aboutdata.py`

 * *Files identical despite different names*

### Comparing `waypaper-2.1/waypaper/app.py` & `waypaper-2.1.1/waypaper/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pathlib import Path
 from PIL import Image
 
 from waypaper.aboutdata import AboutData
 from waypaper.changer import change_wallpaper
 from waypaper.config import Config
 from waypaper.common import get_image_paths, get_random_file
-from waypaper.options import FILL_OPTIONS, BACKEND_OPTIONS, SORT_OPTIONS, SORT_DISPLAYS
+from waypaper.options import FILL_OPTIONS, SORT_OPTIONS, SORT_DISPLAYS
 
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, GdkPixbuf, Gdk, GLib
 
 
 def read_webp_image(image_path):
     """Read webp images using Pillow library and convert it to pixbuf format"""
@@ -54,15 +54,15 @@
 
     def __init__(self, txt):
         super().__init__(title="Waypaper")
         self.cf = Config()
         self.about = AboutData()
         self.txt = txt
         self.check_backends()
-        self.set_default_size(780, 600)
+        self.set_default_size(820, 600)
         self.connect("delete-event", Gtk.main_quit)
         self.selected_index = 0
         self.highlighted_image_row = 0
         self.init_ui()
 
         # Start the image processing in a separate thread:
         threading.Thread(target=self.process_images).start()
@@ -196,15 +196,15 @@
         """Display monitor option if backend is swww"""
         self.options_box.remove(self.monitor_option_combo)
         if self.cf.backend == "swww":
 
             # Check available monitors:
             monitor_names = ["All"]
             try:
-                subprocess.Popen(["swww", "init"])
+                subprocess.Popen(["swww-daemon"])
                 query_output = str(subprocess.check_output(["swww", "query"], encoding='utf-8'))
                 monitors = query_output.split("\n")
                 for monitor in monitors[:-1]:
                     monitor_names.append(monitor.split(':')[0])
             except Exception as e:
                 print(f"{self.txt.err_disp} {e}")
 
@@ -253,15 +253,15 @@
         else:
             pass
 
 
     def process_images(self):
         """Load images from the selected folder, resize them, and arrange into a grid"""
 
-        self.image_paths = get_image_paths(self.cf.backend, self.cf.image_folder, self.cf.include_subfolders, depth=1)
+        self.image_paths = get_image_paths(self.cf.backend, self.cf.image_folder, self.cf.include_subfolders, self.cf.show_hidden, depth=1)
         self.sort_images()
 
         # Show caching label:
         self.loading_label = Gtk.Label(label=self.txt.msg_caching)
         self.bottom_loading_box.add(self.loading_label)
         self.show_all()
 
@@ -432,14 +432,21 @@
             return
         print(self.txt.msg_path, self.cf.selected_wallpaper)
         self.cf.fill_option = self.fill_option_combo.get_active_text() or self.cf.fill_option
         change_wallpaper(self.cf.selected_wallpaper, self.cf, self.cf.selected_monitor, self.txt)
         self.cf.save()
 
 
+    def toggle_hidden_files(self):
+        """Toggle visibility of hidden files"""
+        self.cf.show_hidden = not self.cf.show_hidden
+        threading.Thread(target=self.process_images).start()
+        self.cf.save()
+
+
     def clear_cache(self):
         """Delete cache folder and reprocess the images"""
         try:
             shutil.rmtree(self.cf.cache_dir)
             os.makedirs(self.cf.cache_dir)
         except OSError as e:
             print(f"{self.txt.err_cache} '{self.cf.cache_dir}': {e}")
@@ -453,14 +460,17 @@
 
         elif event.keyval == Gdk.KEY_r:
             self.clear_cache()
 
         elif event.keyval == Gdk.KEY_R:
             self.set_random_wallpaper()
 
+        elif event.keyval in [Gdk.KEY_period]:
+            self.toggle_hidden_files()
+
         elif event.keyval in [Gdk.KEY_h, Gdk.KEY_Left]:
             self.selected_index = max(self.selected_index - 1, 0)
             self.load_image_grid()
             self.scroll_to_selected_image()
 
         elif event.keyval in [Gdk.KEY_j, Gdk.KEY_Down]:
             self.selected_index = min(self.selected_index + 3, len(self.image_paths) - 1)
```

### Comparing `waypaper-2.1/waypaper/changer.py` & `waypaper-2.1.1/waypaper/changer.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         # swaybg backend:
         if cf.backend == "swaybg":
             fill = cf.fill_option.lower()
             try:
                 subprocess.Popen(["killall", "swaybg"])
                 time.sleep(0.005)
             except Exception as e:
-                print(f"{ERR_KILL} {e}")
+                print(f"{txt.err_kill} {e}")
             command = ["swaybg"]
             # if monitor != "All":
                 # command.extend(["-o", monitor])
             command.extend(["-i", image_path])
             command.extend(["-m", fill, "-c", cf.color])
             subprocess.Popen(command)
             print(f"{txt.msg_setwith} {cf.backend}")
@@ -37,16 +37,16 @@
                     }
             fill = fill_types[cf.fill_option.lower()]
             if "swaybg" in cf.installed_backends:
                 try:
                     subprocess.Popen(["killall", "swaybg"])
                     time.sleep(0.005)
                 except Exception as e:
-                    print(f"{ERR_KILL} {e}")
-            subprocess.Popen(["swww", "init"])
+                    print(f"{txt.err_kill} {e}")
+            subprocess.Popen(["swww-daemon"])
             command = ["swww", "img", image_path]
             command.extend(["--resize", fill])
             command.extend(["--fill-color", cf.color])
             command.extend(["--transition-type", cf.swww_transition_type])
             command.extend(["--transition-step", str(cf.swww_transition_step)])
             command.extend(["--transition-angle", str(cf.swww_transition_angle)])
             command.extend(["--transition-duration", str(cf.swww_transition_duration)])
@@ -85,16 +85,14 @@
             print(f"{txt.msg_setwith} {cf.backend}")
 
         else:
             print(f"{txt.err_notsup} {cf.backend}")
 
         # Run a post command:
         if cf.post_command:
-            command = cf.post_command.split(" ")
-            for index, word in enumerate(command):
-                if word == "$wallpaper":
-                    command[index] = image_path
-            subprocess.Popen(command)
-            print(f'{" ".join(command)} executed')
+            modified_image_path = image_path.replace(" ", "\\ ")
+            post_command = cf.post_command.replace("$wallpaper", modified_image_path)
+            subprocess.Popen(post_command, shell=True)
+            print(f'Post command {post_command} executed')
 
     except Exception as e:
         print(f"{txt.err_wall} {e}")
```

### Comparing `waypaper-2.1/waypaper/common.py` & `waypaper-2.1.1/waypaper/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,34 +9,37 @@
 def has_image_extension(file_path, backend):
     """Check if the file has image extension"""
     image_extensions = IMAGE_EXTENSIONS[backend]
     ext = os.path.splitext(file_path)[1].lower()
     return ext in image_extensions
 
 
-def get_image_paths(backend, root_folder, include_subfolders=False, depth=None):
+def get_image_paths(backend, root_folder, include_subfolders=False, include_hidden=False, depth=None):
     """Get a list of file paths depending of weather we include subfolders and how deep we scan"""
     image_paths = []
     for root, directories, files in os.walk(root_folder):
         if not include_subfolders and root != root_folder:
             continue
         if depth is not None and root != root_folder:
             current_depth = root.count(os.path.sep) - str(root_folder).count(os.path.sep)
             if current_depth > depth:
                 continue
         for filename in files:
-            if has_image_extension(filename, backend):
-                image_paths.append(os.path.join(root, filename))
+            if not has_image_extension(filename, backend):
+                continue
+            if filename.startswith('.') and not include_hidden:
+                continue
+            image_paths.append(os.path.join(root, filename))
     return image_paths
 
 
-def get_random_file(backend, folder, include_subfolders):
+def get_random_file(backend, folder, include_subfolders, include_hidden=False):
     """Pick a random file from the folder"""
     try:
-        image_paths = get_image_paths(backend, folder, include_subfolders, depth=1)
+        image_paths = get_image_paths(backend, folder, include_subfolders, include_hidden, depth=1)
         return random.choice(image_paths)
     except:
         return None
 
 
 def check_installed_backends():
     """Check which backends are installed in the system"""
```

### Comparing `waypaper-2.1/waypaper/config.py` & `waypaper-2.1.1/waypaper/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,18 @@
         self.color = "#ffffff"
         self.swww_transition_type = SWWW_TRANSITION_TYPES[0]
         self.swww_transition_step = 90
         self.swww_transition_angle = 0
         self.swww_transition_duration = 2
         self.lang = "en"
         self.monitors = [self.selected_monitor]
-        self.wallpaper = []
+        self.wallpapers = []
         self.post_command = ""
         self.include_subfolders = False
+        self.show_hidden = False
         self.about = AboutData()
         self.cache_dir = user_cache_path(self.about.applicationName())
         self.config_dir = user_config_path(self.about.applicationName())
         self.config_file = self.config_dir / "config.ini"
 
         # Create config and cache folders:
         self.config_dir.mkdir(parents=True, exist_ok=True)
@@ -58,22 +59,23 @@
         self.post_command = config.get("Settings", "post_command", fallback=self.post_command)
         self.swww_transition_type = config.get("Settings", "swww_transition_type", fallback=self.swww_transition_type)
         self.swww_transition_step = config.get("Settings", "swww_transition_step", fallback=self.swww_transition_step)
         self.swww_transition_angle = config.get("Settings", "swww_transition_angle", fallback=self.swww_transition_angle)
         self.swww_transition_duration = config.get("Settings", "swww_transition_duration", fallback=self.swww_transition_duration)
         self.lang = config.get("Settings", "language", fallback=self.lang)
         self.include_subfolders = config.getboolean("Settings", "subfolders", fallback=self.include_subfolders)
+        self.show_hidden = config.getboolean("Settings", "show_hidden", fallback=self.show_hidden)
         self.monitors_str = config.get("Settings", "monitors", fallback=self.selected_monitor, raw=True)
-        self.wallpaper_str = config.get("Settings", "wallpaper", fallback="", raw=True)
+        self.wallpapers_str = config.get("Settings", "wallpaper", fallback="", raw=True)
 
         # Convert strings to lists:
         if self.monitors_str is not None:
             self.monitors = [str(monitor) for monitor in self.monitors_str.split(",")]
-        if self.wallpaper_str is not None:
-            self.wallpaper = [str(paper) for paper in self.wallpaper_str.split(",")]
+        if self.wallpapers_str is not None:
+            self.wallpapers = [str(paper) for paper in self.wallpapers_str.split(",")]
 
     def check_validity(self):
         """Check if the config parameters are valid and correct them if needed"""
         if self.backend not in BACKEND_OPTIONS:
             self.backend = self.installed_backends[0] if self.installed_backends else BACKEND_OPTIONS[0]
         if self.sort_option not in SORT_OPTIONS:
             self.sort_option = SORT_OPTIONS[0]
@@ -91,36 +93,37 @@
 
     def save(self):
         """Update the parameters and save them to the configuration file"""
 
         # If only certain monitor was affected, change only its wallpaper:
         if self.selected_monitor == "All":
             self.monitors = [self.selected_monitor]
-            self.wallpaper = [self.selected_wallpaper]
+            self.wallpapers = [self.selected_wallpaper]
         elif self.selected_monitor in self.monitors:
             index = self.monitors.index(self.selected_monitor)
-            self.wallpaper[index] = self.selected_wallpaper
+            self.wallpapers[index] = self.selected_wallpaper
         else:
             self.monitors.append(self.selected_monitor)
-            self.wallpaper.append(self.selected_wallpaper)
+            self.wallpapers.append(self.selected_wallpaper)
 
         # Write configuration to the file:
         config = configparser.ConfigParser()
         config.read(self.config_file)
         if not config.has_section("Settings"):
             config.add_section("Settings")
         config.set("Settings", "language", self.lang)
         config.set("Settings", "folder", self.image_folder)
-        config.set("Settings", "wallpaper", ",".join(self.wallpaper))
+        config.set("Settings", "wallpaper", ",".join(self.wallpapers))
         config.set("Settings", "backend", self.backend)
         config.set("Settings", "monitors", ",".join(self.monitors))
         config.set("Settings", "fill", self.fill_option)
         config.set("Settings", "sort", self.sort_option)
         config.set("Settings", "color", self.color)
         config.set("Settings", "subfolders", str(self.include_subfolders))
+        config.set("Settings", "show_hidden", str(self.show_hidden))
         config.set("Settings", "post_command", self.post_command)
         config.set("Settings", "swww_transition_type", str(self.swww_transition_type))
         config.set("Settings", "swww_transition_step", str(self.swww_transition_step))
         config.set("Settings", "swww_transition_angle", str(self.swww_transition_angle))
         config.set("Settings", "swww_transition_duration", str(self.swww_transition_duration))
         with open(self.config_file, "w") as configfile:
             config.write(configfile)
```

### Comparing `waypaper-2.1/waypaper/options.py` & `waypaper-2.1.1/waypaper/options.py`

 * *Files identical despite different names*

### Comparing `waypaper-2.1/waypaper/translations.py` & `waypaper-2.1.1/waypaper/translations.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.msg_changefolder = "Change wallpaper folder"
         self.msg_choosefolder = "Please choose a folder"
         self.msg_caching = "Caching wallpapers..."
         self.msg_setwith = "Sent command to set wallpaper was set with"
 
         self.msg_help = "Waypaper's hotkeys:\n\nhjkl - Navigation (←↓↑→)\nf - Change wallpaper folder\n"
         self.msg_help += "g - Scroll to top\nG - Scroll to bottom\nR - Set random wallpaper\nr - Recache wallpapers\n"
-        self.msg_help += "s - Include/exclude images in subfolders\n? - Help\nq - Exit\n\n"
+        self.msg_help += ". - Include/exclude hidden images\ns - Include/exclude images in subfolders\n? - Help\nq - Exit\n\n"
         self.msg_help += self.msg_info
 
         self.err_cache = "Error deleting cache"
         self.err_backend = "Looks like none of the wallpaper backends is installed in the system.\n"
         self.err_backend += "Use your package manager to install at least one of these backends:\n\n"
         self.err_backend += "- swaybg (for Wayland)\n- swww (for Wayland)\n"
         self.err_backend += "- feh (for Xorg)\n- wallutils (for Xorg & Wayland)\n\n"
@@ -70,15 +70,15 @@
         self.msg_changefolder = "Hintergrundbild-Ordner ändern"
         self.msg_choosefolder = "Bitte wählen Sie einen Ordner aus"
         self.msg_caching = "Hintergrundbilder werden zwischengespeichert..."
         self.msg_setwith = "Hintergrundbild wurde mit folgendem Befehl gesetzt"
 
         self.msg_help = "Waypapers Tastenkürzel:\n\nhjkl - Navigation (←↓↑→)\nf - Hintergrundbild-Ordner ändern\n"
         self.msg_help += "g - Zum Anfang scrollen\nG - Zum Ende scrollen\nR - Zufälliges Hintergrundbild\nr - Hintergrundbilder zwischenspeichern\n"
-        self.msg_help += "s - Unterordner mit einbeziehen\n? - Hilfe\nq - Beenden\n\n"
+        self.msg_help += ". - Versteckte Bilder einbeziehen/ausschließen\ns - Unterordner mit einbeziehen\n? - Hilfe\nq - Beenden\n\n"
         self.msg_help += self.msg_info
 
         self.err_cache = "Fehler beim Löschen des Zwischenspeichers"
         self.err_backend = "Es konnte kein Hintergrundbild-Backend gefunden werden.\n"
         self.err_backend += "Installieren Sie mindestens eines der folgenden Backends:\n\n"
         self.err_backend += "- swaybg (für Wayland)\n- swww (für Wayland)\n"
         self.err_backend += "- feh (für Xorg)\n- wallutils (für Xorg & Wayland)\n\n"
@@ -119,15 +119,15 @@
         self.msg_changefolder = "Changer de dossier de papier peint"
         self.msg_choosefolder = "Veuillez choisir un dossier"
         self.msg_caching = "Mise en cache des papiers peints..."
         self.msg_setwith = "La commande envoyée pour définir le papier peint a été définie avec"
 
         self.msg_help = "Raccourcis clavier de Waypaper :\n\nhjkl - Navigation (←↓↑→)\nf - Changer de dossier de papier peint\n"
         self.msg_help += "g - Faire défiler vers le haut\nG - Faire défiler vers le bas\nR - Définir un papier peint aléatoire\nr - Recréer le cache des papiers peints\n"
-        self.msg_help += "s - Inclure/exclure les images des sous-dossiers\n? - Aide\nq - Quitter\n\n"
+        self.msg_help += ". - Inclure/exclure les images cachées\ns - Inclure/exclure les images des sous-dossiers\n? - Aide\nq - Quitter\n\n"
         self.msg_help += self.msg_info
 
         self.err_cache = "Erreur lors de la suppression du cache"
         self.err_backend = "Il semble qu'aucun des backends de papier peint ne soit installé sur le système.\n"
         self.err_backend += "Utilisez votre gestionnaire de paquets pour installer au moins l'un de ces backends :\n\n"
         self.err_backend += "- swaybg (pour Wayland)\n- swww (pour Wayland)\n"
         self.err_backend += "- feh (pour Xorg)\n- wallutils (pour Xorg & Wayland)\n\n"
@@ -168,15 +168,15 @@
         self.msg_changefolder = "Zmień folder z tapetami"
         self.msg_choosefolder = "Proszę wybrać folder"
         self.msg_caching = "Kasowanie tapet..."
         self.msg_setwith = "Wysłano polecenie ustawienia tapety z"
 
         self.msg_help = "Skróty klawiszowe Waypaper:\n\nhjkl - Nawigacja (←↓↑→)\nf - Zmień folder z tapetami\n"
         self.msg_help += "g - Przewiń do góry\nG - Przewiń na dół\nR - Ustaw losową tapetę\nr - Odśwież katalog z tapetami\n"
-        self.msg_help += "s - Dołącz/wyłącz obrazy z podkatalogów\n? - Pomoc\nq - Wyjście\n\n"
+        self.msg_help += ". - Załącz/Wyłącz ukryte obrazy\ns - Dołącz/wyłącz obrazy z podkatalogów\n? - Pomoc\nq - Wyjście\n\n"
         self.msg_help += self.msg_info
 
         self.err_cache = "Błąd podczas usuwania pamięci podręcznej"
         self.err_backend = "Wygląda na to, że żaden z backendów tapet nie jest zainstalowany w systemie.\n"
         self.err_backend += "Użyj menedżera pakietów, aby zainstalować co najmniej jeden z tych backendów:\n\n"
         self.err_backend += "- swaybg (dla Wayland)\n- swww (dla Wayland)\n"
         self.err_backend += "- feh (dla Xorg)\n- wallutils (dla Xorg i Wayland)\n\n"
@@ -217,15 +217,15 @@
         self.msg_changefolder = "Изменить папку с обоями"
         self.msg_choosefolder = "Пожалуйста, выберите папку"
         self.msg_caching = "Кэширование обоев..."
         self.msg_setwith = "Отправлена команда на установку обоев с использованием"
 
         self.msg_help = "Горячие клавиши Waypaper:\n\nhjkl - Навигация (←↓↑→)\nf - Изменить папку с обоями\n"
         self.msg_help += "g - Прокрутка в начало\nG - Прокрутка в конец\nR - Установить случайные обои\nr - Обновить кэш обоев\n"
-        self.msg_help += "s - Включить/отключить изображения в подпапках\n? - Справка\nq - Выход\n\n"
+        self.msg_help += ". - Включить/исключить скрытые файлы \ns - Включить/исключить подпапки\n? - Справка\nq - Выход\n\n"
         self.msg_help += self.msg_info
 
         self.err_cache = "Ошибка при удалении кэша"
         self.err_backend = "Похоже, что ни один из бэкендов для установки обоев не установлен в системе.\n"
         self.err_backend += "Используйте менеджер пакетов для установки хотя бы одного из этих бэкендов:\n\n"
         self.err_backend += "- swaybg (для Wayland)\n- swww (для Wayland)\n"
         self.err_backend += "- feh (для Xorg)\n- wallutils (для Xorg и Wayland)\n\n"
@@ -266,15 +266,15 @@
         self.msg_changefolder = "更改壁纸文件夹"
         self.msg_choosefolder = "请选择一个文件夹"
         self.msg_caching = "缓存壁纸..."
         self.msg_setwith = "发送设置壁纸的命令是用"
 
         self.msg_help = "Waypaper 的热键：\n\nhjkl -导航 (←↓↑→)\nf -更改壁纸文件夹\n"
         self.msg_help += "g -滚动到顶部\nG -滚动到底部\nR -设置随机壁纸\nr -重新缓存壁纸\n"
-        self.msg_help += "s -包含/排除子文件夹中的图像\n？ -帮助\nq -退出\n\n"
+        self.msg_help += ". - 包括/排除隐藏图像\ns -包含/排除子文件夹中的图像\n？ -帮助\nq -退出\n\n"
         self.msg_help += self.msg_info
 
         self.err_cache = "删除缓存时出错"
         self.err_backend = "系统中似乎没有安装壁纸后端。\n"
         self.err_backend += "使用包管理器安装至少以下后端之一：\n\n"
         self.err_backend += "-swaybg (用于 Wayland)\n-swww (用于 Wayland)\n"
         self.err_backend += "-feh (对于 Xorg)\n-wallutils (对于 Xorg 和 Wayland)\n\n"
```

### Comparing `waypaper-2.1/waypaper.egg-info/PKG-INFO` & `waypaper-2.1.1/waypaper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waypaper
-Version: 2.1
+Version: 2.1.1
 Summary: GUI wallpaper setter for Wayland
 Home-page: https://github.com/anufrievroman/waypaper
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -63,14 +63,18 @@
 
 The [waypaper-git](https://aur.archlinux.org/packages/waypaper-git) package is available in AUR, thanks to *metak*. Please upvote to support the project.
 
 #### On NixOS
 
 The `waypaper` package is available thanks to Basil Keeler.
 
+#### On OpenSUSE
+
+Users of OpenSUSE [reported issue with installation](https://github.com/anufrievroman/waypaper/issues/30) via `pipx install waypaper`. This might be resolved by installing the `python311-pycairo-devel` package.
+
 ### Dependencies
 
 - `swww` or `swaybg` or `feh` or `wallutils`
 - gobject python library (it might be called `python-gobject` or `python3-gi` or `python3-gobject` in your package manager.)
 - `python-importlib_metadata`
 - `python-platformdirs`
```

