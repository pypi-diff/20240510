# Comparing `tmp/wei_office_simptool-0.0.7.tar.gz` & `tmp/wei_office_simptool-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wei_office_simptool-0.0.7.tar", last modified: Tue Apr 23 08:59:52 2024, max compression
+gzip compressed data, was "wei_office_simptool-0.0.8.tar", last modified: Fri May 10 07:44:29 2024, max compression
```

## Comparing `wei_office_simptool-0.0.7.tar` & `wei_office_simptool-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 08:59:52.993323 wei_office_simptool-0.0.7/
--rw-rw-rw-   0        0        0     5346 2024-04-23 08:59:52.991309 wei_office_simptool-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4530 2024-04-23 08:08:12.000000 wei_office_simptool-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 08:59:52.993323 wei_office_simptool-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2498 2024-04-23 08:08:12.000000 wei_office_simptool-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 08:59:52.974085 wei_office_simptool-0.0.7/tests/
--rw-rw-rw-   0        0        0     1359 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.7/tests/__init__.py
--rw-rw-rw-   0        0        0     2101 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.7/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 08:59:52.977085 wei_office_simptool-0.0.7/wei_office_simptool/
--rw-rw-rw-   0        0        0     1669 2024-04-19 08:47:36.000000 wei_office_simptool-0.0.7/wei_office_simptool/__init__.py
--rw-rw-rw-   0        0        0    15286 2024-04-23 08:08:12.000000 wei_office_simptool-0.0.7/wei_office_simptool/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 08:59:52.989077 wei_office_simptool-0.0.7/wei_office_simptool.egg-info/
--rw-rw-rw-   0        0        0     5346 2024-04-23 08:59:52.000000 wei_office_simptool-0.0.7/wei_office_simptool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-04-23 08:59:52.000000 wei_office_simptool-0.0.7/wei_office_simptool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 08:59:52.000000 wei_office_simptool-0.0.7/wei_office_simptool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-04-23 08:59:52.000000 wei_office_simptool-0.0.7/wei_office_simptool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-23 08:59:52.000000 wei_office_simptool-0.0.7/wei_office_simptool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 07:44:29.581195 wei_office_simptool-0.0.8/
+-rw-rw-rw-   0        0        0     5924 2024-05-10 07:44:29.578259 wei_office_simptool-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5108 2024-05-10 07:42:24.000000 wei_office_simptool-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-10 07:44:29.581195 wei_office_simptool-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2498 2024-05-10 07:22:33.000000 wei_office_simptool-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 07:44:29.555197 wei_office_simptool-0.0.8/tests/
+-rw-rw-rw-   0        0        0     1359 2024-05-10 02:27:11.000000 wei_office_simptool-0.0.8/tests/__init__.py
+-rw-rw-rw-   0        0        0     2101 2024-05-10 02:27:11.000000 wei_office_simptool-0.0.8/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 07:44:29.558191 wei_office_simptool-0.0.8/wei_office_simptool/
+-rw-rw-rw-   0        0        0     1669 2024-05-10 02:27:11.000000 wei_office_simptool-0.0.8/wei_office_simptool/__init__.py
+-rw-rw-rw-   0        0        0    16396 2024-05-10 07:36:36.000000 wei_office_simptool-0.0.8/wei_office_simptool/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 07:44:29.575199 wei_office_simptool-0.0.8/wei_office_simptool.egg-info/
+-rw-rw-rw-   0        0        0     5924 2024-05-10 07:44:29.000000 wei_office_simptool-0.0.8/wei_office_simptool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-05-10 07:44:29.000000 wei_office_simptool-0.0.8/wei_office_simptool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 07:44:29.000000 wei_office_simptool-0.0.8/wei_office_simptool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-10 07:44:29.000000 wei_office_simptool-0.0.8/wei_office_simptool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-10 07:44:29.000000 wei_office_simptool-0.0.8/wei_office_simptool.egg-info/top_level.txt
```

### Comparing `wei_office_simptool-0.0.7/PKG-INFO` & `wei_office_simptool-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wei_office_simptool
-Version: 0.0.7
+Version: 0.0.8
 Summary: 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换、文件移动等常见功能,实现1到3行代码完成相关处理的快捷操作。
 Home-page: https://github.com/phoenixlucky/wei_office_simptool
 Author: Ethan Wilkins
 Author-email: thisluckyboy@126.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -89,14 +89,26 @@
 # 示例代码
      home_file = pathlib.Path.cwd()
      openfile = pathlib.Path(home_file) / "1.xlsx"
      savefile = pathlib.Path(home_file) / "2.xlsx"
      with OpenExcel(openfile, savefile).my_open() as ws:
          eExcel.fast_write(ws, results, sr, sc, er=0, ec=0, re=0)
 ```
+
+### 2.1 eExcel 类
+创建、写入表
+```bash
+from wei_office_simptool import eExcel
+eExcel(file_name=r"D:\Deskto\1.xlsx")
+#读取
+x=eExcel(file_name=r"D:\Deskto\1.xlsx").excel_read(start_row, start_col, end_row, end_col)
+#写入
+eExcel(file_name=r"D:\Deskto\1.xlsx").excel_write(ws="Sheet1",results, start_row, start_col, end_row, end_col)
+```
+
 ## 3. eSend 类
 用于发送邮件。
 
 ```bash
 from wei_office_simptool import eSend
 
 # 示例代码
@@ -104,32 +116,37 @@
 email_sender.send_email(subject='Your Subject', e_content='Your Email Content', file_paths=['/path/to/file/'], file_names=['attachment.txt'])
 ```
 
 ## 4 DateFormat 类
 用于获取最近的时间处理。
 
 ```bash
-from wei_office_simptool import eDateFormat
+from wei_office_simptool import DateFormat
 
 # 示例代码
 #timeclass:1日期 date 2时间戳 timestamp 3时刻 time 4datetime
 #获取当日的日期字符串
-x=eDateFormat(interval_day=0,timeclass='date').get_timeparameter(Format="%Y-%m-%d")
+x=DateFormat(interval_day=0,timeclass='date').get_timeparameter(Format="%Y-%m-%d")
 print(x)
+
+# 格式化df的表的列属性
+ df = DateFormat(interval_day=0,timeclass='date').datetime_standar(df, '日期')
 ```
 
 ## 5 FileManagement 类
 用于文件移动并且重命名。
 ```bash
 #latest_folder2 当前目录
 #destination_directory 目标目录
 #target_files2 文件名
 #add_prefix 重命名去除数字
 #file_type 文件类型
-copy_files(latest_folder2, destination_directory, target_files2, rename=add_prefix,file_type="xls")
+FileManagement().copy_files(latest_folder2, destination_directory, target_files2, rename=True,file_type="xls")
+#寻找最新文件夹
+latest_folder = FileManagement().find_latest_folder(base_directory)
 ```
 
 ## 贡献
 #### 有任何问题或建议，请提出 issue。欢迎贡献代码！
 
 Copyright (c) 2024 The Python Packaging Authority
```

### Comparing `wei_office_simptool-0.0.7/README.md` & `wei_office_simptool-0.0.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -69,14 +69,26 @@
 # 示例代码
      home_file = pathlib.Path.cwd()
      openfile = pathlib.Path(home_file) / "1.xlsx"
      savefile = pathlib.Path(home_file) / "2.xlsx"
      with OpenExcel(openfile, savefile).my_open() as ws:
          eExcel.fast_write(ws, results, sr, sc, er=0, ec=0, re=0)
 ```
+
+### 2.1 eExcel 类
+创建、写入表
+```bash
+from wei_office_simptool import eExcel
+eExcel(file_name=r"D:\Deskto\1.xlsx")
+#读取
+x=eExcel(file_name=r"D:\Deskto\1.xlsx").excel_read(start_row, start_col, end_row, end_col)
+#写入
+eExcel(file_name=r"D:\Deskto\1.xlsx").excel_write(ws="Sheet1",results, start_row, start_col, end_row, end_col)
+```
+
 ## 3. eSend 类
 用于发送邮件。
 
 ```bash
 from wei_office_simptool import eSend
 
 # 示例代码
@@ -84,32 +96,37 @@
 email_sender.send_email(subject='Your Subject', e_content='Your Email Content', file_paths=['/path/to/file/'], file_names=['attachment.txt'])
 ```
 
 ## 4 DateFormat 类
 用于获取最近的时间处理。
 
 ```bash
-from wei_office_simptool import eDateFormat
+from wei_office_simptool import DateFormat
 
 # 示例代码
 #timeclass:1日期 date 2时间戳 timestamp 3时刻 time 4datetime
 #获取当日的日期字符串
-x=eDateFormat(interval_day=0,timeclass='date').get_timeparameter(Format="%Y-%m-%d")
+x=DateFormat(interval_day=0,timeclass='date').get_timeparameter(Format="%Y-%m-%d")
 print(x)
+
+# 格式化df的表的列属性
+ df = DateFormat(interval_day=0,timeclass='date').datetime_standar(df, '日期')
 ```
 
 ## 5 FileManagement 类
 用于文件移动并且重命名。
 ```bash
 #latest_folder2 当前目录
 #destination_directory 目标目录
 #target_files2 文件名
 #add_prefix 重命名去除数字
 #file_type 文件类型
-copy_files(latest_folder2, destination_directory, target_files2, rename=add_prefix,file_type="xls")
+FileManagement().copy_files(latest_folder2, destination_directory, target_files2, rename=True,file_type="xls")
+#寻找最新文件夹
+latest_folder = FileManagement().find_latest_folder(base_directory)
 ```
 
 ## 贡献
 #### 有任何问题或建议，请提出 issue。欢迎贡献代码！
 
 Copyright (c) 2024 The Python Packaging Authority
```

### Comparing `wei_office_simptool-0.0.7/setup.py` & `wei_office_simptool-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 @email:thisluckyboy@126.com
 """
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='wei_office_simptool',
-    version='0.0.7',
+    version='0.0.8',
     author="Ethan Wilkins",
     author_email="thisluckyboy@126.com",
     description="一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换、文件移动等常见功能,实现1到3行代码完成相关处理的快捷操作。",  # 包的简述
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/phoenixlucky/wei_office_simptool",
     packages=find_packages(),
```

### Comparing `wei_office_simptool-0.0.7/tests/__init__.py` & `wei_office_simptool-0.0.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.7/tests/test_utils.py` & `wei_office_simptool-0.0.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.7/wei_office_simptool/__init__.py` & `wei_office_simptool-0.0.8/wei_office_simptool/__init__.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.7/wei_office_simptool/utils.py` & `wei_office_simptool-0.0.8/wei_office_simptool/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 import smtplib
 import time
 from contextlib import contextmanager
 from email.header import Header
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from functools import wraps
+from pathlib import Path
 
 import mysql.connector
 import openpyxl
 import pandas as pd
 import pymysql
 from openpyxl import load_workbook
 
@@ -173,25 +174,32 @@
     def __init__(self):
         pass
 
     def add_prefix(self,filename,file_type):
         pattern = r'[\u4e00-\u9fa5]+'
         matches = re.findall(pattern, filename)[0]
         return f"{matches}.{file_type}"
-    def copy_files(self,src_dir, dest_dir, target_files, rename=None,file_type="xls"):
+    def copy_files(self,src_dir, dest_dir, target_files, rename=False,file_type="xls"):
         for target_file in target_files:
             source_path = os.path.join(src_dir, target_file)
-            destination_file = rename(target_file,file_type) if rename else target_file
+            destination_file = self.add_prefix(target_file,file_type) if rename else target_file
             destination_path = os.path.join(dest_dir, destination_file)
             if os.path.exists(source_path):
                 shutil.copy(source_path, destination_path)
                 print(f"File {target_file} copied from {source_path} to {destination_path}")
             else:
                 print(f"Source file {target_file} not found in the latest folder.")
 
+    def find_latest_folder(self,base_dir):
+        folders = [f for f in Path(base_dir).iterdir() if f.is_dir()]
+        if not folders:
+            return None
+        latest_folder = max(folders, key=os.path.getctime)
+        return latest_folder
+
 class MySQLDatabase:
     def __init__(self, config):
         self.config = config
         self.connection = None
         self.connect()
 
     def connect(self):
@@ -358,26 +366,46 @@
             realtime = time.strftime(Format, time.localtime(time.time()))
         elif self.timeclass=='datetime':
             realtime= datetime.datetime.fromtimestamp(int(time.time()))
         else:
             raise TypeError("你输入的参数不合理!")
         return realtime
 
+    def datetime_standar(self,df, colname):
+    #处理表格的列文本时间格式
+        if self.timeclass == 'date':
+            df[colname] = pd.to_datetime(df[colname]).dt.date
+        elif self.timeclass == 'time':
+            formats = ['%Y-%m-%d', '%H:%M:%S', '%Y-%m-%d %H:%M:%S']
+            for fmt in formats:
+                try:
+                    df[colname] = pd.to_datetime(df[colname], format=fmt)
+                    break
+                except ValueError:
+                    continue
+            else:
+                print(f"Column {colname} cannot be parsed with the provided formats.")
+        else:
+            print("Invalid type. Choose either 'date' or 'time'.")
+        return df
+
 
 class eExcel:
-    def __init__(self, visible=1, file_name=None):
+    def __init__(self, file_name=None):
         self.file_name = file_name
         if not pathlib.Path(file_name).exists():
             self.create_new_excel(file_name)
         self.wb = openpyxl.load_workbook(file_name)
         self.ws = self.wb.active
 
     @staticmethod
     def create_new_excel(file_name):
         wb = openpyxl.Workbook()
+        sheet = wb.active
+        sheet.title = 'sheet1'  # 设置工作表的名称为sheet1
         wb.save(file_name)
 
     @staticmethod
     def excel_write(ws, results, start_row, start_col, end_row, end_col):
         for i, row in enumerate(range(start_row, end_row + 1)):
             for j, value in enumerate(range(start_col, end_col + 1)):
                 ws.cell(row=row, column=value, value=results[i][j])
```

### Comparing `wei_office_simptool-0.0.7/wei_office_simptool.egg-info/PKG-INFO` & `wei_office_simptool-0.0.8/wei_office_simptool.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wei_office_simptool
-Version: 0.0.7
+Version: 0.0.8
 Summary: 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换、文件移动等常见功能,实现1到3行代码完成相关处理的快捷操作。
 Home-page: https://github.com/phoenixlucky/wei_office_simptool
 Author: Ethan Wilkins
 Author-email: thisluckyboy@126.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -89,14 +89,26 @@
 # 示例代码
      home_file = pathlib.Path.cwd()
      openfile = pathlib.Path(home_file) / "1.xlsx"
      savefile = pathlib.Path(home_file) / "2.xlsx"
      with OpenExcel(openfile, savefile).my_open() as ws:
          eExcel.fast_write(ws, results, sr, sc, er=0, ec=0, re=0)
 ```
+
+### 2.1 eExcel 类
+创建、写入表
+```bash
+from wei_office_simptool import eExcel
+eExcel(file_name=r"D:\Deskto\1.xlsx")
+#读取
+x=eExcel(file_name=r"D:\Deskto\1.xlsx").excel_read(start_row, start_col, end_row, end_col)
+#写入
+eExcel(file_name=r"D:\Deskto\1.xlsx").excel_write(ws="Sheet1",results, start_row, start_col, end_row, end_col)
+```
+
 ## 3. eSend 类
 用于发送邮件。
 
 ```bash
 from wei_office_simptool import eSend
 
 # 示例代码
@@ -104,32 +116,37 @@
 email_sender.send_email(subject='Your Subject', e_content='Your Email Content', file_paths=['/path/to/file/'], file_names=['attachment.txt'])
 ```
 
 ## 4 DateFormat 类
 用于获取最近的时间处理。
 
 ```bash
-from wei_office_simptool import eDateFormat
+from wei_office_simptool import DateFormat
 
 # 示例代码
 #timeclass:1日期 date 2时间戳 timestamp 3时刻 time 4datetime
 #获取当日的日期字符串
-x=eDateFormat(interval_day=0,timeclass='date').get_timeparameter(Format="%Y-%m-%d")
+x=DateFormat(interval_day=0,timeclass='date').get_timeparameter(Format="%Y-%m-%d")
 print(x)
+
+# 格式化df的表的列属性
+ df = DateFormat(interval_day=0,timeclass='date').datetime_standar(df, '日期')
 ```
 
 ## 5 FileManagement 类
 用于文件移动并且重命名。
 ```bash
 #latest_folder2 当前目录
 #destination_directory 目标目录
 #target_files2 文件名
 #add_prefix 重命名去除数字
 #file_type 文件类型
-copy_files(latest_folder2, destination_directory, target_files2, rename=add_prefix,file_type="xls")
+FileManagement().copy_files(latest_folder2, destination_directory, target_files2, rename=True,file_type="xls")
+#寻找最新文件夹
+latest_folder = FileManagement().find_latest_folder(base_directory)
 ```
 
 ## 贡献
 #### 有任何问题或建议，请提出 issue。欢迎贡献代码！
 
 Copyright (c) 2024 The Python Packaging Authority
```

