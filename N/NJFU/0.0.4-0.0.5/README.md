# Comparing `tmp/NJFU-0.0.4.tar.gz` & `tmp/NJFU-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NJFU-0.0.4.tar", last modified: Wed May  8 10:57:18 2024, max compression
+gzip compressed data, was "NJFU-0.0.5.tar", last modified: Fri May 10 03:07:21 2024, max compression
```

## Comparing `NJFU-0.0.4.tar` & `NJFU-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 10:57:18.516259 NJFU-0.0.4/
-drwxrwxrwx   0        0        0        0 2024-05-08 10:57:18.512272 NJFU-0.0.4/NJFU/
--rw-rw-rw-   0        0        0       87 2024-05-08 08:29:37.000000 NJFU-0.0.4/NJFU/__init__.py
--rw-rw-rw-   0        0        0       61 2024-05-07 09:27:16.000000 NJFU-0.0.4/NJFU/hello.py
--rw-rw-rw-   0        0        0    19420 2024-05-08 10:54:30.000000 NJFU-0.0.4/NJFU/utils.py
--rw-rw-rw-   0        0        0     9577 2024-05-08 10:54:30.000000 NJFU-0.0.4/NJFU/yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:57:18.515262 NJFU-0.0.4/NJFU.egg-info/
--rw-rw-rw-   0        0        0      900 2024-05-08 10:57:18.000000 NJFU-0.0.4/NJFU.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2024-05-08 10:57:18.000000 NJFU-0.0.4/NJFU.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 10:57:18.000000 NJFU-0.0.4/NJFU.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-08 10:57:18.000000 NJFU-0.0.4/NJFU.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      900 2024-05-08 10:57:18.516259 NJFU-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-08 10:57:18.517256 NJFU-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1060 2024-05-08 10:57:14.000000 NJFU-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:07:21.870636 NJFU-0.0.5/
+drwxrwxrwx   0        0        0        0 2024-05-10 03:07:21.866650 NJFU-0.0.5/NJFU/
+-rw-rw-rw-   0        0        0       87 2024-05-08 08:29:37.000000 NJFU-0.0.5/NJFU/__init__.py
+-rw-rw-rw-   0        0        0       61 2024-05-07 09:27:16.000000 NJFU-0.0.5/NJFU/hello.py
+-rw-rw-rw-   0        0        0    19420 2024-05-08 10:54:30.000000 NJFU-0.0.5/NJFU/utils.py
+-rw-rw-rw-   0        0        0     9645 2024-05-10 03:03:13.000000 NJFU-0.0.5/NJFU/yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:07:21.869640 NJFU-0.0.5/NJFU.egg-info/
+-rw-rw-rw-   0        0        0      900 2024-05-10 03:07:21.000000 NJFU-0.0.5/NJFU.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2024-05-10 03:07:21.000000 NJFU-0.0.5/NJFU.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 03:07:21.000000 NJFU-0.0.5/NJFU.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-10 03:07:21.000000 NJFU-0.0.5/NJFU.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      900 2024-05-10 03:07:21.870636 NJFU-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-10 03:07:21.870636 NJFU-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1060 2024-05-10 03:07:19.000000 NJFU-0.0.5/setup.py
```

### Comparing `NJFU-0.0.4/NJFU/utils.py` & `NJFU-0.0.5/NJFU/utils.py`

 * *Files identical despite different names*

### Comparing `NJFU-0.0.4/NJFU/yolo.py` & `NJFU-0.0.5/NJFU/yolo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import os
 import cv2
 import argparse
+import xml.etree.ElementTree as ET
+import numpy as np
 from utils import DataAugmentForObjectDetection, ToolHelper, show_pic
 
 
-def TXT2XML(input_txt_dir, output_xml_dir, image_dir, class_txt):
+def TXT2XML(input_txt_dir, output_xml_dir, image_dir, class_txt, pic_type):
     # 获取txt文件的目录列表
     txt_files = os.listdir(input_txt_dir)
     # 获取图像的目录列表
     image_files = os.listdir(image_dir)
     image_infos = []
     for txt_file in txt_files:
         file_name, file_ext = os.path.splitext(txt_file)
         for image_file in image_files:
             images = []
             image_name, image_ext = os.path.splitext(image_file)
-            if image_ext == '.jpg':
+            if image_ext == pic_type:
                 # 判断图像名是否与txt文件名相同
                 if image_name == file_name:
                     images.append(image_file)
                     # 读取txt文件中的标注信息
                     with open(os.path.join(input_txt_dir, txt_file), 'r') as f:
                         bboxes = []
                         for line in f.readlines():
```

### Comparing `NJFU-0.0.4/NJFU.egg-info/PKG-INFO` & `NJFU-0.0.5/NJFU.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NJFU
-Version: 0.0.4
+Version: 0.0.5
 Summary: NJFU
 Home-page: https://github.com/
 Author: XHF
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 2
```

### Comparing `NJFU-0.0.4/PKG-INFO` & `NJFU-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NJFU
-Version: 0.0.4
+Version: 0.0.5
 Summary: NJFU
 Home-page: https://github.com/
 Author: XHF
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 2
```

### Comparing `NJFU-0.0.4/setup.py` & `NJFU-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 
 setuptools.setup(
     name="NJFU",
-    version="0.0.4",
+    version="0.0.5",
     author="XHF",
 
     description="NJFU",
 
-    Long_description_content_type="text/markdown",
+    Long_description_content_type="Tool for NJFU",
     url="https://github.com/",
     packages=setuptools.find_packages(),
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Programming Language :: Python :: 2",
```

