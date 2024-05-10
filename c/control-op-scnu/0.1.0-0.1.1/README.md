# Comparing `tmp/control_op_scnu-0.1.0.tar.gz` & `tmp/control_op_scnu-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control_op_scnu-0.1.0.tar", last modified: Fri May 10 13:52:07 2024, max compression
+gzip compressed data, was "control_op_scnu-0.1.1.tar", last modified: Fri May 10 14:18:27 2024, max compression
```

## Comparing `control_op_scnu-0.1.0.tar` & `control_op_scnu-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 13:52:07.672084 control_op_scnu-0.1.0/
--rw-rw-rw-   0        0        0      409 2024-05-10 13:52:07.671084 control_op_scnu-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 13:52:07.640658 control_op_scnu-0.1.0/control_op_scnu/
--rw-rw-rw-   0        0        0     9553 2024-05-02 16:29:46.000000 control_op_scnu-0.1.0/control_op_scnu/__init__.py
--rw-rw-rw-   0        0        0     8264 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/file_operation.py
--rw-rw-rw-   0        0        0    28521 2024-05-06 13:49:28.000000 control_op_scnu-0.1.0/control_op_scnu/gpio.py
--rw-rw-rw-   0        0        0     1494 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/jiami.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:52:07.659072 control_op_scnu-0.1.0/control_op_scnu/lcd/
--rw-rw-rw-   0        0        0     6200 2024-04-29 14:22:37.000000 control_op_scnu-0.1.0/control_op_scnu/lcd/LCD_2inch4.py
--rw-rw-rw-   0        0        0       22 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/lcd/__init__.py
--rw-rw-rw-   0        0        0     4040 2024-05-05 06:57:21.000000 control_op_scnu-0.1.0/control_op_scnu/lcd/lcdconfig.py
--rw-rw-rw-   0        0        0     6097 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/machine_learning.py
--rw-rw-rw-   0        0        0     5183 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/maths.py
--rw-rw-rw-   0        0        0    21274 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/shijue0.py
--rw-rw-rw-   0        0        0    46326 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/shijue1.py
--rw-rw-rw-   0        0        0     7021 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/shijue2.py
--rw-rw-rw-   0        0        0     2595 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/unique.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:52:07.670086 control_op_scnu-0.1.0/control_op_scnu/util/
--rw-rw-rw-   0        0        0     1067 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/util/Voice_line_patrol.py
--rw-rw-rw-   0        0        0        0 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/util/__init__.py
--rw-rw-rw-   0        0        0     2008 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/util/all_path.py
--rw-rw-rw-   0        0        0     7185 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/util/auto_poetry.py
--rw-rw-rw-   0        0        0     2220 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/util/checkLibVersion.py
--rw-rw-rw-   0        0        0     4681 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/util/download.py
--rw-rw-rw-   0        0        0     9933 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/util/flappy_bird.py
--rw-rw-rw-   0        0        0     7711 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/util/local_yuyin.py
--rw-rw-rw-   0        0        0     9935 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/util/ml_tool.py
--rw-rw-rw-   0        0        0     3948 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/util/number_convert.py
--rw-rw-rw-   0        0        0     1886 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/util/opencv_tool.py
--rw-rw-rw-   0        0        0     3327 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/util/playsound_change.py
--rw-rw-rw-   0        0        0     5428 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/util/word_cloud.py
--rw-rw-rw-   0        0        0    31160 2024-04-29 12:52:38.000000 control_op_scnu-0.1.0/control_op_scnu/yuyin.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:52:07.670086 control_op_scnu-0.1.0/control_op_scnu.egg-info/
--rw-rw-rw-   0        0        0      409 2024-05-10 13:52:07.000000 control_op_scnu-0.1.0/control_op_scnu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1077 2024-05-10 13:52:07.000000 control_op_scnu-0.1.0/control_op_scnu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 13:52:07.000000 control_op_scnu-0.1.0/control_op_scnu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-10 13:52:07.000000 control_op_scnu-0.1.0/control_op_scnu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-10 13:52:07.000000 control_op_scnu-0.1.0/control_op_scnu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 13:52:07.672084 control_op_scnu-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      743 2024-05-10 13:52:04.000000 control_op_scnu-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:18:27.059492 control_op_scnu-0.1.1/
+-rw-rw-rw-   0        0        0      416 2024-05-10 14:18:27.058491 control_op_scnu-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 14:18:27.038493 control_op_scnu-0.1.1/control_op_scnu/
+-rw-rw-rw-   0        0        0     9553 2024-05-02 16:29:46.000000 control_op_scnu-0.1.1/control_op_scnu/__init__.py
+-rw-rw-rw-   0        0        0     8264 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/file_operation.py
+-rw-rw-rw-   0        0        0    28521 2024-05-06 13:49:28.000000 control_op_scnu-0.1.1/control_op_scnu/gpio.py
+-rw-rw-rw-   0        0        0     1494 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/jiami.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:18:27.048491 control_op_scnu-0.1.1/control_op_scnu/lcd/
+-rw-rw-rw-   0        0        0     6200 2024-04-29 14:22:37.000000 control_op_scnu-0.1.1/control_op_scnu/lcd/LCD_2inch4.py
+-rw-rw-rw-   0        0        0       22 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/lcd/__init__.py
+-rw-rw-rw-   0        0        0     4040 2024-05-05 06:57:21.000000 control_op_scnu-0.1.1/control_op_scnu/lcd/lcdconfig.py
+-rw-rw-rw-   0        0        0     6097 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/machine_learning.py
+-rw-rw-rw-   0        0        0     5183 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/maths.py
+-rw-rw-rw-   0        0        0    21274 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/shijue0.py
+-rw-rw-rw-   0        0        0    46326 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/shijue1.py
+-rw-rw-rw-   0        0        0     7021 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/shijue2.py
+-rw-rw-rw-   0        0        0     2595 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/unique.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:18:27.057498 control_op_scnu-0.1.1/control_op_scnu/util/
+-rw-rw-rw-   0        0        0     1067 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/util/Voice_line_patrol.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/util/__init__.py
+-rw-rw-rw-   0        0        0     2008 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/util/all_path.py
+-rw-rw-rw-   0        0        0     7185 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/util/auto_poetry.py
+-rw-rw-rw-   0        0        0     2220 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/util/checkLibVersion.py
+-rw-rw-rw-   0        0        0     4681 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/util/download.py
+-rw-rw-rw-   0        0        0     9933 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/util/flappy_bird.py
+-rw-rw-rw-   0        0        0     7711 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/util/local_yuyin.py
+-rw-rw-rw-   0        0        0     9935 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/util/ml_tool.py
+-rw-rw-rw-   0        0        0     3948 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/util/number_convert.py
+-rw-rw-rw-   0        0        0     1886 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/util/opencv_tool.py
+-rw-rw-rw-   0        0        0     3327 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/util/playsound_change.py
+-rw-rw-rw-   0        0        0     5428 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/util/word_cloud.py
+-rw-rw-rw-   0        0        0    31160 2024-04-29 12:52:38.000000 control_op_scnu-0.1.1/control_op_scnu/yuyin.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:18:27.058491 control_op_scnu-0.1.1/control_op_scnu.egg-info/
+-rw-rw-rw-   0        0        0      416 2024-05-10 14:18:26.000000 control_op_scnu-0.1.1/control_op_scnu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1077 2024-05-10 14:18:26.000000 control_op_scnu-0.1.1/control_op_scnu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 14:18:26.000000 control_op_scnu-0.1.1/control_op_scnu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-10 14:18:26.000000 control_op_scnu-0.1.1/control_op_scnu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-10 14:18:26.000000 control_op_scnu-0.1.1/control_op_scnu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 14:18:27.059492 control_op_scnu-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      750 2024-05-10 14:18:07.000000 control_op_scnu-0.1.1/setup.py
```

### Comparing `control_op_scnu-0.1.0/control_op_scnu/__init__.py` & `control_op_scnu-0.1.1/control_op_scnu/__init__.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/file_operation.py` & `control_op_scnu-0.1.1/control_op_scnu/file_operation.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/gpio.py` & `control_op_scnu-0.1.1/control_op_scnu/gpio.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/jiami.py` & `control_op_scnu-0.1.1/control_op_scnu/jiami.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/lcd/LCD_2inch4.py` & `control_op_scnu-0.1.1/control_op_scnu/lcd/LCD_2inch4.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/lcd/lcdconfig.py` & `control_op_scnu-0.1.1/control_op_scnu/lcd/lcdconfig.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/machine_learning.py` & `control_op_scnu-0.1.1/control_op_scnu/machine_learning.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/maths.py` & `control_op_scnu-0.1.1/control_op_scnu/maths.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/shijue0.py` & `control_op_scnu-0.1.1/control_op_scnu/shijue0.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/shijue1.py` & `control_op_scnu-0.1.1/control_op_scnu/shijue1.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/shijue2.py` & `control_op_scnu-0.1.1/control_op_scnu/shijue2.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/unique.py` & `control_op_scnu-0.1.1/control_op_scnu/unique.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/util/Voice_line_patrol.py` & `control_op_scnu-0.1.1/control_op_scnu/util/Voice_line_patrol.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/util/all_path.py` & `control_op_scnu-0.1.1/control_op_scnu/util/all_path.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/util/auto_poetry.py` & `control_op_scnu-0.1.1/control_op_scnu/util/auto_poetry.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/util/checkLibVersion.py` & `control_op_scnu-0.1.1/control_op_scnu/util/checkLibVersion.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/util/download.py` & `control_op_scnu-0.1.1/control_op_scnu/util/download.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/util/flappy_bird.py` & `control_op_scnu-0.1.1/control_op_scnu/util/flappy_bird.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/util/local_yuyin.py` & `control_op_scnu-0.1.1/control_op_scnu/util/local_yuyin.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/util/ml_tool.py` & `control_op_scnu-0.1.1/control_op_scnu/util/ml_tool.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/util/number_convert.py` & `control_op_scnu-0.1.1/control_op_scnu/util/number_convert.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/util/opencv_tool.py` & `control_op_scnu-0.1.1/control_op_scnu/util/opencv_tool.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/util/playsound_change.py` & `control_op_scnu-0.1.1/control_op_scnu/util/playsound_change.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/util/word_cloud.py` & `control_op_scnu-0.1.1/control_op_scnu/util/word_cloud.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu/yuyin.py` & `control_op_scnu-0.1.1/control_op_scnu/yuyin.py`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/control_op_scnu.egg-info/SOURCES.txt` & `control_op_scnu-0.1.1/control_op_scnu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `control_op_scnu-0.1.0/setup.py` & `control_op_scnu-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='control_op_scnu',  # 库的名字
-    version='0.1.0',  # 版本号，遵循语义化版本控制
+    version='0.1.1',  # 版本号，遵循语义化版本控制
     packages=find_packages(),  # 自动发现并包含所有包
     description='服务于机器人部',  # 简短描述
 
     author='cpw',  # 作者名
     author_email='1994777538@qq.com',  # 作者邮箱
     url='https://github.com/cpw041130/control_op_scnu',  # 项目主页
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],  # 分类标签
     install_requires=[  # 依赖列表
-        'dependency1',
+        'dependency1>=0.1.0',
         'dependency2>=1.0.0',
     ],
 )
```

