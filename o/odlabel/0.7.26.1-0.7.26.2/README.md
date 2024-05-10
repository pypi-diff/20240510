# Comparing `tmp/odlabel-0.7.26.1.tar.gz` & `tmp/odlabel-0.7.26.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odlabel-0.7.26.1.tar", last modified: Wed May  8 19:14:51 2024, max compression
+gzip compressed data, was "odlabel-0.7.26.2.tar", last modified: Fri May 10 15:39:38 2024, max compression
```

## Comparing `odlabel-0.7.26.1.tar` & `odlabel-0.7.26.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-08 19:14:51.875652 odlabel-0.7.26.1/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    34273 2024-05-06 11:36:33.000000 odlabel-0.7.26.1/LICENSE
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     7818 2024-05-08 19:14:51.875652 odlabel-0.7.26.1/PKG-INFO
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     7054 2024-05-08 19:12:44.000000 odlabel-0.7.26.1/README.md
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-08 19:14:51.875652 odlabel-0.7.26.1/app/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-05 13:42:42.000000 odlabel-0.7.26.1/app/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-0.7.26.1/app/main.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    29628 2024-05-06 11:07:09.000000 odlabel-0.7.26.1/app/main_window.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-08 19:14:51.875652 odlabel-0.7.26.1/app/workers/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:08.000000 odlabel-0.7.26.1/app/workers/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-02 17:12:53.000000 odlabel-0.7.26.1/app/workers/chart_worker.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    14360 2024-05-05 23:39:38.000000 odlabel-0.7.26.1/app/workers/detection_worker.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-08 19:14:51.875652 odlabel-0.7.26.1/app/workers/utils/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-0.7.26.1/app/workers/utils/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    10458 2024-05-02 20:55:30.000000 odlabel-0.7.26.1/app/workers/utils/chart_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     6216 2024-05-05 19:35:10.000000 odlabel-0.7.26.1/app/workers/utils/detection_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1044 2024-05-02 17:12:49.000000 odlabel-0.7.26.1/app/workers/utils/draw_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-0.7.26.1/app/workers/utils/write_utils.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-08 19:14:51.875652 odlabel-0.7.26.1/odlabel.egg-info/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     7818 2024-05-08 19:14:51.000000 odlabel-0.7.26.1/odlabel.egg-info/PKG-INFO
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      520 2024-05-08 19:14:51.000000 odlabel-0.7.26.1/odlabel.egg-info/SOURCES.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-08 19:14:51.000000 odlabel-0.7.26.1/odlabel.egg-info/dependency_links.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       49 2024-05-08 19:14:51.000000 odlabel-0.7.26.1/odlabel.egg-info/entry_points.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       89 2024-05-08 19:14:51.000000 odlabel-0.7.26.1/odlabel.egg-info/requires.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        4 2024-05-08 19:14:51.000000 odlabel-0.7.26.1/odlabel.egg-info/top_level.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      275 2024-05-08 19:14:51.879652 odlabel-0.7.26.1/setup.cfg
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1268 2024-05-08 19:12:05.000000 odlabel-0.7.26.1/setup.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-10 15:39:38.123205 odlabel-0.7.26.2/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    34273 2024-05-06 11:36:33.000000 odlabel-0.7.26.2/LICENSE
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     7818 2024-05-10 15:39:38.123205 odlabel-0.7.26.2/PKG-INFO
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     7054 2024-05-08 19:12:44.000000 odlabel-0.7.26.2/README.md
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-10 15:39:38.119205 odlabel-0.7.26.2/app/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-09 20:45:02.000000 odlabel-0.7.26.2/app/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-0.7.26.2/app/main.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    29628 2024-05-09 20:46:40.000000 odlabel-0.7.26.2/app/main_window.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-10 15:39:38.119205 odlabel-0.7.26.2/app/workers/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:08.000000 odlabel-0.7.26.2/app/workers/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-09 20:44:28.000000 odlabel-0.7.26.2/app/workers/chart_worker.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    14405 2024-05-10 15:31:20.000000 odlabel-0.7.26.2/app/workers/detection_worker.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-10 15:39:38.119205 odlabel-0.7.26.2/app/workers/utils/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-0.7.26.2/app/workers/utils/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    10458 2024-05-02 20:55:30.000000 odlabel-0.7.26.2/app/workers/utils/chart_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     6216 2024-05-10 15:15:58.000000 odlabel-0.7.26.2/app/workers/utils/detection_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1911 2024-05-10 15:39:29.000000 odlabel-0.7.26.2/app/workers/utils/draw_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-0.7.26.2/app/workers/utils/write_utils.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-10 15:39:38.123205 odlabel-0.7.26.2/odlabel.egg-info/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     7818 2024-05-10 15:39:38.000000 odlabel-0.7.26.2/odlabel.egg-info/PKG-INFO
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      520 2024-05-10 15:39:38.000000 odlabel-0.7.26.2/odlabel.egg-info/SOURCES.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-10 15:39:38.000000 odlabel-0.7.26.2/odlabel.egg-info/dependency_links.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       49 2024-05-10 15:39:38.000000 odlabel-0.7.26.2/odlabel.egg-info/entry_points.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       89 2024-05-10 15:39:38.000000 odlabel-0.7.26.2/odlabel.egg-info/requires.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        4 2024-05-10 15:39:38.000000 odlabel-0.7.26.2/odlabel.egg-info/top_level.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      275 2024-05-10 15:39:38.123205 odlabel-0.7.26.2/setup.cfg
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1268 2024-05-10 15:19:59.000000 odlabel-0.7.26.2/setup.py
```

### Comparing `odlabel-0.7.26.1/LICENSE` & `odlabel-0.7.26.2/LICENSE`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.1/PKG-INFO` & `odlabel-0.7.26.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odlabel
-Version: 0.7.26.1
+Version: 0.7.26.2
 Summary: A tool for object detection, labeling and visualization
 Home-page: https://github.com/Ziad-Algrafi/odlabel
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `odlabel-0.7.26.1/README.md` & `odlabel-0.7.26.2/README.md`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.1/app/main_window.py` & `odlabel-0.7.26.2/app/main_window.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.1/app/workers/chart_worker.py` & `odlabel-0.7.26.2/app/workers/chart_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.1/app/workers/detection_worker.py` & `odlabel-0.7.26.2/app/workers/detection_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         self.classes = classes
         self.device = device
         self.use_sahi = use_sahi
         self.slice_size = slice_size
         self._terminate_event = threading.Event()
         self.train_detections = []
         self.val_detections = []
+        self.class_colors = {}
 
         self.log_queue: Union[Queue, None] = None
         self.output_image_queue: Union[Queue, None] = None
         self.progress_queue: Union[Queue, None] = None
         self.show_error_queue: Union[Queue, None] = None
 
     def get_image_files(self):
@@ -194,15 +195,15 @@
         if img is None:
             return
 
         if detections:
             output_img = draw_boxes_on_image(
                 annotated_frame,
                 detections,
-                img,
+                self.class_colors,
                 os.path.join(detected_image_dir, image_file),
             )
 
             output_img_path = os.path.join(detected_image_dir, image_file)
             cv.imwrite(output_img_path, output_img)
 
             self.save_format_results(detections, labels_dir, image_file, i)
```

### Comparing `odlabel-0.7.26.1/app/workers/utils/chart_utils.py` & `odlabel-0.7.26.2/app/workers/utils/chart_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.1/app/workers/utils/detection_utils.py` & `odlabel-0.7.26.2/app/workers/utils/detection_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.1/app/workers/utils/write_utils.py` & `odlabel-0.7.26.2/app/workers/utils/write_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.1/odlabel.egg-info/PKG-INFO` & `odlabel-0.7.26.2/odlabel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odlabel
-Version: 0.7.26.1
+Version: 0.7.26.2
 Summary: A tool for object detection, labeling and visualization
 Home-page: https://github.com/Ziad-Algrafi/odlabel
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `odlabel-0.7.26.1/odlabel.egg-info/SOURCES.txt` & `odlabel-0.7.26.2/odlabel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.1/setup.py` & `odlabel-0.7.26.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="odlabel",
-    version="0.7.26.1",
+    version="0.7.26.2",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "customtkinter",
         "ultralytics",
         "matplotlib",
         "numpy",
```

