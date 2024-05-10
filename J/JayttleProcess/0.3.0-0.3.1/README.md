# Comparing `tmp/JayttleProcess-0.3.0-py3-none-any.whl.zip` & `tmp/JayttleProcess-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 62494 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat     2978 b- defN 24-Apr-29 13:43 JayttleProcess/CommonDecorator.py
--rw-rw-rw-  2.0 fat    10785 b- defN 24-Apr-26 14:47 JayttleProcess/ComputerControl.py
+Zip file size: 64918 bytes, number of entries: 15
+-rw-rw-rw-  2.0 fat     2978 b- defN 24-May-10 14:16 JayttleProcess/CommonDecorator.py
+-rw-rw-rw-  2.0 fat    10769 b- defN 24-May-10 14:16 JayttleProcess/ComputerControl.py
 -rw-rw-rw-  2.0 fat      613 b- defN 24-Apr-08 05:57 JayttleProcess/EntertainmentCode.py
--rw-rw-rw-  2.0 fat     6834 b- defN 24-Apr-29 06:01 JayttleProcess/FTPCommonUse.py
--rw-rw-rw-  2.0 fat     5650 b- defN 24-Apr-24 02:33 JayttleProcess/JsonCommonManage.py
+-rw-rw-rw-  2.0 fat    16839 b- defN 24-May-10 14:16 JayttleProcess/FTPCommonUse.py
+-rw-rw-rw-  2.0 fat     5650 b- defN 24-May-10 14:16 JayttleProcess/JsonCommonManage.py
 -rw-rw-rw-  2.0 fat     3461 b- defN 24-Apr-28 07:21 JayttleProcess/MachineLearning.py
--rw-rw-rw-  2.0 fat    39584 b- defN 24-Apr-24 13:25 JayttleProcess/RinexCommonManage.py
+-rw-rw-rw-  2.0 fat    39584 b- defN 24-May-10 14:16 JayttleProcess/RinexCommonManage.py
 -rw-rw-rw-  2.0 fat    34687 b- defN 24-Apr-29 13:43 JayttleProcess/SQLCommonUse.py
--rw-rw-rw-  2.0 fat    16735 b- defN 24-May-07 05:12 JayttleProcess/TBCProcessCsv.py
--rw-rw-rw-  2.0 fat   124974 b- defN 24-May-06 10:35 JayttleProcess/TimeSeriesDataMethod.py
+-rw-rw-rw-  2.0 fat    16735 b- defN 24-May-10 14:17 JayttleProcess/TBCProcessCsv.py
+-rw-rw-rw-  2.0 fat   124974 b- defN 24-May-10 14:17 JayttleProcess/TimeSeriesDataMethod.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-14 14:39 JayttleProcess/__init__.py
--rw-rw-rw-  2.0 fat      601 b- defN 24-May-07 07:40 JayttleProcess-0.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 07:40 JayttleProcess-0.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-May-07 07:40 JayttleProcess-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1312 b- defN 24-May-07 07:40 JayttleProcess-0.3.0.dist-info/RECORD
-15 files, 248321 bytes uncompressed, 60304 bytes compressed:  75.7%
+-rw-rw-rw-  2.0 fat      596 b- defN 24-May-10 14:17 JayttleProcess-0.3.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-10 14:17 JayttleProcess-0.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-May-10 14:17 JayttleProcess-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1313 b- defN 24-May-10 14:17 JayttleProcess-0.3.1.dist-info/RECORD
+15 files, 258306 bytes uncompressed, 62728 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: JayttleProcess/TimeSeriesDataMethod.py
 Comment: 
 
 Filename: JayttleProcess/__init__.py
 Comment: 
 
-Filename: JayttleProcess-0.3.0.dist-info/METADATA
+Filename: JayttleProcess-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: JayttleProcess-0.3.0.dist-info/WHEEL
+Filename: JayttleProcess-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: JayttleProcess-0.3.0.dist-info/top_level.txt
+Filename: JayttleProcess-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: JayttleProcess-0.3.0.dist-info/RECORD
+Filename: JayttleProcess-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## JayttleProcess/ComputerControl.py

```diff
@@ -182,23 +182,20 @@
     move_and_click(27, 1572)#菜单
     move_and_click(582, 1500)#菜单
     time.sleep(1)
     move_and_click(592, 1433)#关机
     move_and_click(592, 1433)#关机
 
 
-def TBC_auto_Process():
+def TBC_auto_Process(Merge_path , save_path):
     window_region_保存 = (1625, 567, 37, 20)
     window_region_输入= (1590, 950, 35, 16)
     # 目标文件夹路径
-    folder_path = r"D:\Ropeway\FTPMerge"
     # 获取目标文件夹中所有文件夹的名字
-    subdirectories = get_subdirectories_with_no_csv_without03(folder_path)
-
-
+    subdirectories = get_subdirectories_with_no_csv_without03(Merge_path)
     for directory in subdirectories:
         exit_for_loop = False  # 标志，用于指示是否退出外部循环
         ensure_no_input_data()
         move_and_click(87, 31)#本地
         time.sleep(1) #等待
         move_and_click(39, 74)     #tbc-输入
         time.sleep(1) #等待
@@ -258,15 +255,15 @@
         move_and_click(96, 73)#输出菜单
         time.sleep(1) #等待
         move_and_click(54, 244) #单击R031点
         move_and_click(2179, 449) #单击到文件名的初始
         time.sleep(1) #等待
         move_and_click_with_shift(2474, 447) #拖动并全选文件名
         time.sleep(1) #等待
-        type_string(f"D:\\Ropeway\\FTPcsv2\\{directory}.csv") # 输入文件夹名字
+        type_string(f"D:\\Ropeway\\{save_path}\\TBC\\{directory}.csv") # 输入文件夹名字
         time.sleep(1) #等待D
         move_and_click(2436, 1511)#输出栏里的保存
         time.sleep(1) #等待
         move_and_click(168, 290) #单击第一个文件
         time.sleep(0.5) #等待
         move_and_click_with_shift(147, 376) #拖动并点击最后一个文件
         time.sleep(0.5) #等待
```

## JayttleProcess/FTPCommonUse.py

```diff
@@ -1,13 +1,16 @@
 import os
 from ftplib import FTP
 import json
 import datetime
 from dataclasses import dataclass
 import JayttleProcess.CommonDecorator as ComD
+from JayttleProcess import RinexCommonManage
+from JayttleProcess import ComputerControl
+from JayttleProcess.RinexCommonManage import *
 
 
 class FTPConfig:
     def __init__(self, json_file_path: str):
         # 确保 JSON 文件存在
         if not os.path.exists(json_file_path):
             raise FileNotFoundError(f"指定的 JSON 文件不存在: {json_file_path}")
@@ -20,15 +23,14 @@
         ftp_options = self.options.get('FtpOptions', {})
         self.ftp_address = ftp_options.get('Address')
         self.ftp_port = ftp_options.get('Port')
         self.ftp_username = ftp_options.get('UserName')
         self.ftp_password = ftp_options.get('Password')
         self.root_folder = self.options.get('RootFolder')
 
-
     def __str__(self):
         # 返回对象的字符串表示
         return f"FTPConfig(Address={self.ftp_address}, Port={self.ftp_port}, UserName={self.ftp_username}, RootFolder={self.root_folder})"
 
 
 @ComD.log_function_call
 def check_FTP_file() -> None:
@@ -98,14 +100,15 @@
         print(f"发生错误: {e}")
         return False
 
     finally:
         # 关闭FTP连接
         ftp.quit()
 
+
 def download_files_from_ftp(ftp_config: FTPConfig, 
                             remote_folder: str, 
                             files_to_download: list[str], 
                             local_save_path: str) -> bool:
     try:
         # 连接到FTP服务器
         ftp = FTP()
@@ -164,18 +167,209 @@
     files_to_download = [file.strip() for file in files_to_download]
     # 获取文件名的前四个字符并处理
     target_folder = process_string(os.path.basename(txt_file_path)[:4])
     # 使用 FTPConfig 对象下载文件
     success = download_files_from_ftp(ftp_config, remote_folder=target_folder, files_to_download=files_to_download, local_save_path=local_save_path)
     return success
 
+def copy_files(from_folder: str, to_folder: str, prefix: str) -> None:
+    """将指定文件夹中以指定前缀开头的文件复制到目标文件夹中."""
+    for file_name in os.listdir(from_folder):
+        if file_name.startswith(prefix):
+            source_file = os.path.join(from_folder, file_name)
+            destination_file = os.path.join(to_folder, file_name)
+            # 检查目标文件夹中是否已经存在相同的文件
+            if not os.path.exists(destination_file):
+                shutil.copy(source_file, destination_file)
+
+@ComD.log_function_call
+def Process_Copy(isFirst: bool, toDownload_path: str, merge_path: str) -> None:
+    """处理第一部分数据."""
+    if not isFirst:
+        for filename in os.listdir(toDownload_path):
+            # 获取文件名的前四个字符
+            first_four_characters = filename[:4]
+            if first_four_characters in ("B011", "B021"):  # 使用 in 检查多个条件
+                toDownload_file = os.path.join(toDownload_path, filename)
+                # 读取指定的 txt 文件
+                with open(toDownload_file, 'r') as txt_file:
+                    files_to_download: list[str] = txt_file.readlines()
+                # 去除每行末尾的换行符
+                files_to_download = [file.strip() for file in files_to_download]
+                from_copy_folder = r"D:\Ropeway\R051_1619\FTPMerge"
+                merge_folders: list[str] = os.listdir(from_copy_folder)
+                file_data = {}
+                # 遍历 files_to_download 列表并检查是否需要移除元素
+                for file_to_download in files_to_download.copy():
+                    third_part: str = file_to_download.split('_')[2]  # 获取文件名中的第三部分
+                    first_part: str = file_to_download.split('_')[0][:4]
+                    isNeedRemove: bool = False
+                    if third_part in merge_folders and first_part == first_four_characters:
+                        isNeedRemove = True
+                        from_copy_merge_folder: str = os.path.join(from_copy_folder, third_part)
+                        to_merge_folder = os.path.join(merge_path, third_part)
+                        os.makedirs(to_merge_folder, exist_ok=True)
+                        copy_files(from_copy_merge_folder, to_merge_folder, first_four_characters)
+                    if not isNeedRemove:
+                        date_part: str = file_to_download.split('_')[2][:7]
+                        if date_part not in file_data:
+                            file_data[date_part] = []
+                        file_data[date_part].append(file_to_download.strip())
+                
+                # 删除长度不满指定个数的条目
+                specified_length = 8  # 指定的长度
+                to_remove = [date_part for date_part, files_list in file_data.items() if len(files_list) < specified_length]
+                for date_part in to_remove:
+                    del file_data[date_part]
+
+                # 将更新后的 file_data 保存回原始的文本文件中
+                with open(toDownload_file, 'w') as txt_file:
+                    for files_list in file_data.values():
+                        txt_file.write('\n'.join(files_list) + '\n')
+
+
+
+
+@ComD.log_function_call
+def Process_Part1(output_file_path, specified_marker_names, start_hour, end_hour):
+    """
+    1.完成  _toDownload.txt中存放需下载文件
+    """
+    # 指定文件夹
+    directory_path = r"D:\Ropeway\GNSS\FTP_File_Situation"
+    # 要读取得所有FTP文件的情况
+    file_list_path = os.path.join(directory_path, "all_files.txt")
+    # 读取rnx文件信息 list[RinexFileInfo]
+    rinex_files_info: list[RinexFileInfo] = RinexCommonManage.read_rinex_files_info(file_list_path)
+
+    # # 指定时间范围
+    # start_hour= 16
+    # end_hour = 19
+    # 统计每天指定时间范围内文件的数量，并按日期和标记站名返回文件数的字典。
+    files_in_hour_range: dict[datetime.date, dict[str, int]] = RinexCommonManage.count_files_in_hour_range(rinex_files_info, start_hour, end_hour)
+    # 要检查的文件数
+    specified_count = (end_hour - start_hour + 1) * 2
+    # 查找指定标记站名文件数同时为8的日期列表
+    dates_with_specific_count:list[datetime.date] = RinexCommonManage.find_dates_with_specific_file_count(files_in_hour_range, specified_marker_names, specified_count)
+    """
+    dates_with_specific_count 就是想要下载的日期列表
+    """
+    # 要下载的文件名放到 _toDownload.txt中
+    for item in specified_marker_names:
+        to_download_file_name = os.path.join(output_file_path, f"{item}_toDownload.txt")
+        marker_name = item
+        RinexCommonManage.write_rinex_files_to_txt(rinex_files_info, marker_name, dates_with_specific_count, to_download_file_name, start_hour, end_hour)
+
+
+@ComD.log_function_call
+def Process_Part2(toDownload_path, local_save_path):
+    """
+    2.完成指定文件的下载工作
+    """
+    # json文件
+    json_file_path = r'D:\Program Files (x86)\Software\OneDrive\PyPackages\options.json'
+    # 读取json文件里的FTPConfig
+    ftp_config = FTPConfig(json_file_path)
+    # 下载的目的地
+    # 遍历文件夹中的文件
+    for filename in os.listdir(toDownload_path):
+        # 获取文件名的前四个字符
+        first_four_characters = filename[:4]
+        # 构建要保存的本地路径
+        save_folder_path = os.path.join(local_save_path, first_four_characters)
+        # 检查本地路径是否存在，如果不存在，则创建
+        if not os.path.exists(save_folder_path):
+            os.makedirs(save_folder_path)
+        RinexCommonManage.delete_small_files(save_folder_path, 0.1)
+        if download_files_from_ftp_by_txt(ftp_config, os.path.join(toDownload_path, filename), save_folder_path):
+            print("文件下载成功！")
+        else:
+            print("文件下载失败。")
+
+
+@ComD.log_function_call
+def Process_Part3(local_save_path):
+    """
+    3.解压缩 .Z格式文件
+    4.文件转换 CRX2RNX.exe
+    """
+    for foldername in os.listdir(local_save_path):
+        save_folder_path = os.path.join(local_save_path, foldername)
+        # 解压缩文件
+        RinexCommonManage.unzip_folder_path(folder_path = save_folder_path)
+        print("文件解压成功！")
+        # 读取文件夹中crx格式的文件 并且没有同名的rnx格式的文件
+        to_convert_crx_files: list[RinexFileInfo] = RinexCommonManage.get_rnx_files_crx(save_folder_path)
+        # CRX2RNX 文件转换
+        RinexCommonManage.crx_to_rnx(to_convert_crx_files)
+        print("文件转换成功！")
+
+@ComD.log_function_call
+def Process_Part4(local_save_path, merge_path):
+    """
+    5.合并rnx文件
+    6.对MO文件 markername的修改
+    executed in 3999.1432s
+    """
+    for foldername in os.listdir(local_save_path):
+        save_folder_path = os.path.join(local_save_path, foldername)    
+        # 用日期来作为key值,将同一天的数据存放在一起
+        rnx_files: dict[datetime.date, list[RinexFileInfo]] = RinexCommonManage.get_rnx_files_dict_date(save_folder_path)
+        to_process_rnx_file: list[list[RinexFileInfo]] = []
+        for start_date, rinex_list in rnx_files.items():
+            o_files: list[RinexFileInfo] = [rnx_file for rnx_file in rinex_list if rnx_file.file_type == RinexFileType.O]
+            n_files: list[RinexFileInfo] = [rnx_file for rnx_file in rinex_list if rnx_file.file_type == RinexFileType.N]
+            to_process_rnx_file.append(o_files)
+            to_process_rnx_file.append(n_files)
+        # 合并文件
+        RinexCommonManage.merge_files_threadpool(to_process_rnx_file, merge_path, 4)
+        # 遍历合并文件的保存地址 下的所有文件夹里面的 _MO.rnx文件预处理
+        RinexCommonManage.process_rnx_files(merge_path)
+    
+
+@ComD.log_function_call
+def Process_Check(toDownload_path, local_save_path):
+    file_lines_mapping = RinexCommonManage.count_lines_in_each_txt_file(toDownload_path)
+    for file_name, num_lines in file_lines_mapping.items():
+        print(f"文件 '{file_name}' 的行数为: {num_lines}")
+    folder_file_count = RinexCommonManage.count_files_in_folders(local_save_path)
+    for folder_name, file_count in folder_file_count.items():
+        print(f"文件夹 '{folder_name}' 中包含 {file_count} 个文件.")
+
+@ComD.log_function_call
+def Process_in_one_step():
+    base_marker_names = ['B011', 'B021']
+    root_folder = f"D:\Ropeway" # 存储软件运行的根目录
+    to_process_marker_names = ['R052', 'R071']
+#    to_process_marker_names = ['R031', 'R032', 'R051', 'R052', 'R071', 'R072', 'R081', 'R082']
+    # 指定时间范围
+    start_hour= 16
+    end_hour = 19
+    TBC_Process = False
+    for item in to_process_marker_names:
+        folder_name = f"{item}_{start_hour}{end_hour}"
+        folder_path = os.path.join(root_folder, folder_name)
+        os.makedirs(folder_path, exist_ok=True)
+        toDownload_folder = os.path.join(folder_path, 'toDownload')
+        os.makedirs(toDownload_folder, exist_ok=True)
+        FTP_folder = os.path.join(folder_path, 'FTP')
+        os.makedirs(FTP_folder, exist_ok=True)
+        FTPMerge_folder = os.path.join(folder_path, 'FTPMerge')
+        os.makedirs(FTPMerge_folder, exist_ok=True)
+        TBC_folder = os.path.join(folder_path, 'TBC')
+        os.makedirs(TBC_folder, exist_ok=True)
+        base_marker_names.append(item)
+        Process_Part1(toDownload_folder, base_marker_names, start_hour, end_hour)
+        Process_Copy(False, toDownload_folder ,FTPMerge_folder)
+
+        # Process_Part2(toDownload_folder, FTP_folder)
+        # Process_Part3(FTP_folder)
+        # Process_Part4(FTP_folder, FTPMerge_folder)
+        # Process_Check(toDownload_folder, FTP_folder)
+        if TBC_Process:
+            ComputerControl.TBC_auto_Process(FTPMerge_folder, folder_name)
+        base_marker_names.remove(item)
+        
 
-# # 示例使用
-# json_file_path = r'D:\Program Files (x86)\Software\OneDrive\PyPackages\options.json'
-# ftp_config = FTPConfig(json_file_path)
-# txt_file_path = r'D:\Ropeway\GNSS\R031_output_B021.txt'
-# local_save_path = r'D:\Ropeway\GNSS\FTP\B021'
-
-# if download_files_from_ftp_by_txt(ftp_config, txt_file_path, local_save_path):
-#     print("文件下载成功！")
-# else:
-#     print("文件下载失败。")
+def shut_down_tbc():
+    ComputerControl.auto_turn_off_TBC()
+    ComputerControl.auto_turn_off()
```

## Comparing `JayttleProcess-0.3.0.dist-info/METADATA` & `JayttleProcess-0.3.1.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: JayttleProcess
-Version: 0.3.0
-Summary: modifty time:2024-05-07 21:25
+Version: 0.3.1
+Summary: modifty time:2024-05-10 
  en: Data Process;
  zh_CN:数据处理的方法
 Home-page: UNKNOWN
 Author: Jayttle
 Author-email: 294448068@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
```

