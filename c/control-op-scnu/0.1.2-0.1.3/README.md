# Comparing `tmp/control-op-scnu-0.1.2.tar.gz` & `tmp/control-op-scnu-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-op-scnu-0.1.2.tar", last modified: Fri May 10 14:26:23 2024, max compression
+gzip compressed data, was "control-op-scnu-0.1.3.tar", last modified: Fri May 10 14:33:11 2024, max compression
```

## Comparing `control-op-scnu-0.1.2.tar` & `control-op-scnu-0.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 14:26:23.319222 control-op-scnu-0.1.2/
--rw-rw-rw-   0        0        0      413 2024-05-10 14:26:23.318221 control-op-scnu-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-10 14:25:00.000000 control-op-scnu-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 14:26:23.290826 control-op-scnu-0.1.2/control_op_scnu/
--rw-rw-rw-   0        0        0     9553 2024-05-02 16:29:46.000000 control-op-scnu-0.1.2/control_op_scnu/__init__.py
--rw-rw-rw-   0        0        0     8264 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/file_operation.py
--rw-rw-rw-   0        0        0    28521 2024-05-06 13:49:28.000000 control-op-scnu-0.1.2/control_op_scnu/gpio.py
--rw-rw-rw-   0        0        0     1494 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/jiami.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:26:23.306953 control-op-scnu-0.1.2/control_op_scnu/lcd/
--rw-rw-rw-   0        0        0     6200 2024-04-29 14:22:37.000000 control-op-scnu-0.1.2/control_op_scnu/lcd/LCD_2inch4.py
--rw-rw-rw-   0        0        0       22 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/lcd/__init__.py
--rw-rw-rw-   0        0        0     4040 2024-05-05 06:57:21.000000 control-op-scnu-0.1.2/control_op_scnu/lcd/lcdconfig.py
--rw-rw-rw-   0        0        0     6097 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/machine_learning.py
--rw-rw-rw-   0        0        0     5183 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/maths.py
--rw-rw-rw-   0        0        0    21274 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/shijue0.py
--rw-rw-rw-   0        0        0    46326 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/shijue1.py
--rw-rw-rw-   0        0        0     7021 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/shijue2.py
--rw-rw-rw-   0        0        0     2595 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/unique.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:26:23.316221 control-op-scnu-0.1.2/control_op_scnu/util/
--rw-rw-rw-   0        0        0     1067 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/util/Voice_line_patrol.py
--rw-rw-rw-   0        0        0        0 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/util/__init__.py
--rw-rw-rw-   0        0        0     2008 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/util/all_path.py
--rw-rw-rw-   0        0        0     7185 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/util/auto_poetry.py
--rw-rw-rw-   0        0        0     2220 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/util/checkLibVersion.py
--rw-rw-rw-   0        0        0     4681 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/util/download.py
--rw-rw-rw-   0        0        0     9933 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/util/flappy_bird.py
--rw-rw-rw-   0        0        0     7711 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/util/local_yuyin.py
--rw-rw-rw-   0        0        0     9935 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/util/ml_tool.py
--rw-rw-rw-   0        0        0     3948 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/util/number_convert.py
--rw-rw-rw-   0        0        0     1886 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/util/opencv_tool.py
--rw-rw-rw-   0        0        0     3327 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/util/playsound_change.py
--rw-rw-rw-   0        0        0     5428 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/util/word_cloud.py
--rw-rw-rw-   0        0        0    31160 2024-04-29 12:52:38.000000 control-op-scnu-0.1.2/control_op_scnu/yuyin.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:26:23.317222 control-op-scnu-0.1.2/control_op_scnu.egg-info/
--rw-rw-rw-   0        0        0      413 2024-05-10 14:26:23.000000 control-op-scnu-0.1.2/control_op_scnu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1049 2024-05-10 14:26:23.000000 control-op-scnu-0.1.2/control_op_scnu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 14:26:23.000000 control-op-scnu-0.1.2/control_op_scnu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-10 14:26:23.000000 control-op-scnu-0.1.2/control_op_scnu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 14:26:23.319222 control-op-scnu-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1038 2024-05-10 14:26:15.000000 control-op-scnu-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:33:11.308733 control-op-scnu-0.1.3/
+-rw-rw-rw-   0        0        0      413 2024-05-10 14:33:11.307736 control-op-scnu-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-10 14:25:00.000000 control-op-scnu-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 14:33:11.278731 control-op-scnu-0.1.3/control/
+-rw-rw-rw-   0        0        0     9553 2024-05-02 16:29:46.000000 control-op-scnu-0.1.3/control/__init__.py
+-rw-rw-rw-   0        0        0     8264 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/file_operation.py
+-rw-rw-rw-   0        0        0    28521 2024-05-06 13:49:28.000000 control-op-scnu-0.1.3/control/gpio.py
+-rw-rw-rw-   0        0        0     1494 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/jiami.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:33:11.280732 control-op-scnu-0.1.3/control/lcd/
+-rw-rw-rw-   0        0        0     6200 2024-04-29 14:22:37.000000 control-op-scnu-0.1.3/control/lcd/LCD_2inch4.py
+-rw-rw-rw-   0        0        0       22 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/lcd/__init__.py
+-rw-rw-rw-   0        0        0     4040 2024-05-05 06:57:21.000000 control-op-scnu-0.1.3/control/lcd/lcdconfig.py
+-rw-rw-rw-   0        0        0     6097 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/machine_learning.py
+-rw-rw-rw-   0        0        0     5183 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/maths.py
+-rw-rw-rw-   0        0        0    21274 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/shijue0.py
+-rw-rw-rw-   0        0        0    46326 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/shijue1.py
+-rw-rw-rw-   0        0        0     7021 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/shijue2.py
+-rw-rw-rw-   0        0        0     2595 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/unique.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:33:11.289732 control-op-scnu-0.1.3/control/util/
+-rw-rw-rw-   0        0        0     1067 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/util/Voice_line_patrol.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/util/__init__.py
+-rw-rw-rw-   0        0        0     2008 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/util/all_path.py
+-rw-rw-rw-   0        0        0     7185 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/util/auto_poetry.py
+-rw-rw-rw-   0        0        0     2220 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/util/checkLibVersion.py
+-rw-rw-rw-   0        0        0     4681 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/util/download.py
+-rw-rw-rw-   0        0        0     9933 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/util/flappy_bird.py
+-rw-rw-rw-   0        0        0     7711 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/util/local_yuyin.py
+-rw-rw-rw-   0        0        0     9935 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/util/ml_tool.py
+-rw-rw-rw-   0        0        0     3948 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/util/number_convert.py
+-rw-rw-rw-   0        0        0     1886 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/util/opencv_tool.py
+-rw-rw-rw-   0        0        0     3327 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/util/playsound_change.py
+-rw-rw-rw-   0        0        0     5428 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/util/word_cloud.py
+-rw-rw-rw-   0        0        0    31160 2024-04-29 12:52:38.000000 control-op-scnu-0.1.3/control/yuyin.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:33:11.306731 control-op-scnu-0.1.3/control_op_scnu.egg-info/
+-rw-rw-rw-   0        0        0      413 2024-05-10 14:33:11.000000 control-op-scnu-0.1.3/control_op_scnu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      833 2024-05-10 14:33:11.000000 control-op-scnu-0.1.3/control_op_scnu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 14:33:11.000000 control-op-scnu-0.1.3/control_op_scnu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-10 14:33:11.000000 control-op-scnu-0.1.3/control_op_scnu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 14:33:11.308733 control-op-scnu-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1038 2024-05-10 14:33:08.000000 control-op-scnu-0.1.3/setup.py
```

### Comparing `control-op-scnu-0.1.2/control_op_scnu/__init__.py` & `control-op-scnu-0.1.3/control/__init__.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/file_operation.py` & `control-op-scnu-0.1.3/control/file_operation.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/gpio.py` & `control-op-scnu-0.1.3/control/gpio.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/jiami.py` & `control-op-scnu-0.1.3/control/jiami.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/lcd/LCD_2inch4.py` & `control-op-scnu-0.1.3/control/lcd/LCD_2inch4.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/lcd/lcdconfig.py` & `control-op-scnu-0.1.3/control/lcd/lcdconfig.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/machine_learning.py` & `control-op-scnu-0.1.3/control/machine_learning.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/maths.py` & `control-op-scnu-0.1.3/control/maths.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/shijue0.py` & `control-op-scnu-0.1.3/control/shijue0.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/shijue1.py` & `control-op-scnu-0.1.3/control/shijue1.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/shijue2.py` & `control-op-scnu-0.1.3/control/shijue2.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/unique.py` & `control-op-scnu-0.1.3/control/unique.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/util/Voice_line_patrol.py` & `control-op-scnu-0.1.3/control/util/Voice_line_patrol.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/util/all_path.py` & `control-op-scnu-0.1.3/control/util/all_path.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/util/auto_poetry.py` & `control-op-scnu-0.1.3/control/util/auto_poetry.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/util/checkLibVersion.py` & `control-op-scnu-0.1.3/control/util/checkLibVersion.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/util/download.py` & `control-op-scnu-0.1.3/control/util/download.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/util/flappy_bird.py` & `control-op-scnu-0.1.3/control/util/flappy_bird.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/util/local_yuyin.py` & `control-op-scnu-0.1.3/control/util/local_yuyin.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/util/ml_tool.py` & `control-op-scnu-0.1.3/control/util/ml_tool.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/util/number_convert.py` & `control-op-scnu-0.1.3/control/util/number_convert.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/util/opencv_tool.py` & `control-op-scnu-0.1.3/control/util/opencv_tool.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/util/playsound_change.py` & `control-op-scnu-0.1.3/control/util/playsound_change.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/util/word_cloud.py` & `control-op-scnu-0.1.3/control/util/word_cloud.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/control_op_scnu/yuyin.py` & `control-op-scnu-0.1.3/control/yuyin.py`

 * *Files identical despite different names*

### Comparing `control-op-scnu-0.1.2/setup.py` & `control-op-scnu-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="control-op-scnu",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.1.2",  # 包版本号，便于维护版本
+    version="0.1.3",  # 包版本号，便于维护版本
     author="cpw",  # 作者，可以写自己的姓名
     author_email="1994777538@qq.com",  # 作者联系方式，可写自己的邮箱地址
     description="A small example package",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/cpw041130/control_op_scnu",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

