# Comparing `tmp/blues_lib-1.0.0.tar.gz` & `tmp/blues_lib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\blues_lib-1.0.0.tar", last modified: Sat Apr 20 14:16:33 2024, max compression
+gzip compressed data, was "dist\blues_lib-1.0.1.tar", last modified: Thu May  9 18:10:12 2024, max compression
```

## Comparing `blues_lib-1.0.0.tar` & `blues_lib-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 14:16:33.802184 blues_lib-1.0.0/
--rw-rw-rw-   0        0        0      495 2024-04-20 14:16:33.802184 blues_lib-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-04-20 14:16:24.000000 blues_lib-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 14:16:33.792679 blues_lib-1.0.0/blues_lib.egg-info/
--rw-rw-rw-   0        0        0      495 2024-04-20 14:16:33.000000 blues_lib-1.0.0/blues_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-20 14:16:33.000000 blues_lib-1.0.0/blues_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 14:16:33.000000 blues_lib-1.0.0/blues_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-20 14:16:33.000000 blues_lib-1.0.0/blues_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-20 14:16:33.000000 blues_lib-1.0.0/blues_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-20 14:16:33.797952 blues_lib-1.0.0/blues_util/
--rw-rw-rw-   0        0        0     3960 2024-04-20 10:31:15.000000 blues_lib-1.0.0/blues_util/BluesFiler.py
--rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.0.0/blues_util/BluesImager.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.0/blues_util/__init__.py
--rw-rw-rw-   0        0        0       86 2024-04-20 14:16:33.803178 blues_lib-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      366 2024-04-20 14:15:53.000000 blues_lib-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:10:12.885818 blues_lib-1.0.1/
+-rw-rw-rw-   0        0        0     1065 2024-05-09 18:10:12.886844 blues_lib-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2024-05-07 10:02:36.000000 blues_lib-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 18:10:12.855414 blues_lib-1.0.1/blues_lib.egg-info/
+-rw-rw-rw-   0        0        0     1065 2024-05-09 18:10:12.000000 blues_lib-1.0.1/blues_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2024-05-09 18:10:12.000000 blues_lib-1.0.1/blues_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 18:10:12.000000 blues_lib-1.0.1/blues_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-09 18:10:12.000000 blues_lib-1.0.1/blues_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-09 18:10:12.000000 blues_lib-1.0.1/blues_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 18:10:12.864993 blues_lib-1.0.1/blues_sql/
+-rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.0.1/blues_sql/BluesMySQLExecutor.py
+-rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.0.1/blues_sql/BluesSQLConvertor.py
+-rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.0.1/blues_sql/BluesSQLExecutor.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.0.1/blues_sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:10:12.883654 blues_lib-1.0.1/blues_util/
+-rw-rw-rw-   0        0        0     1506 2024-05-09 17:16:52.000000 blues_lib-1.0.1/blues_util/BluesConsole.py
+-rw-rw-rw-   0        0        0      766 2024-04-26 16:50:11.000000 blues_lib-1.0.1/blues_util/BluesDateTime.py
+-rw-rw-rw-   0        0        0     4955 2024-04-26 16:18:11.000000 blues_lib-1.0.1/blues_util/BluesFiler.py
+-rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.0.1/blues_util/BluesImager.py
+-rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.0.1/blues_util/BluesLogger.py
+-rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.0.1/blues_util/BluesMailer.py
+-rw-rw-rw-   0        0        0     1713 2024-05-07 09:54:17.000000 blues_lib-1.0.1/blues_util/BluesPowerShell.py
+-rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.0.1/blues_util/BluesType.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.0.1/blues_util/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-05-09 18:10:12.887846 blues_lib-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      366 2024-05-09 18:09:22.000000 blues_lib-1.0.1/setup.py
```

### Comparing `blues_lib-1.0.0/blues_util/BluesFiler.py` & `blues_lib-1.0.1/blues_util/BluesFiler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import os,requests
+from datetime import datetime,timedelta
 
 class BluesFiler:
   
   @classmethod
   def removedirs(cls,directory):
     '''
     @description Remove all child dir and files
     @param {string} directory 
     '''
+    removed_count = 0
     for root, dirs, files in os.walk(directory):
       for file in files:
         os.remove(os.path.join(root, file))
+        removed_count +=1
       for dir in dirs:
         os.rmdir(os.path.join(root, dir))
+        removed_count +=1
+    return removed_count
 
   @classmethod
   def download(cls,urls,directory,success=None,error=None):
     '''
     @description Download multi files
     @param {list} urls files' remote url
     @param {string} directory : Local directory to save the downloaded files
@@ -141,8 +146,33 @@
     copy_name = new_name if new_name else original_name
     if prefix:
       copy_name = prefix+separator+copy_name
     if suffix:
       copy_name = copy_name+separator+suffix
     path_slices[-1]=copy_name
     copy_path='/'.join(path_slices)
-    return copy_path
+    return copy_path
+
+  @classmethod
+  def removefiles(cls,directory,retention_days=7):
+    '''
+    @description : clear files before n days
+    @param {str} directory
+    @param {int} retention_days : default 7
+    @returns {int} deleted files count
+    '''
+    # 转换天数到时间间隔
+    threshold = datetime.now() - timedelta(days=retention_days)
+    removed_count = 0
+    # 遍历目录
+    for item in os.scandir(directory):
+      try:
+        # 获取文件的最后修改时间
+        file_modified_time = datetime.fromtimestamp(os.path.getmtime(item.path))
+        # 如果文件的最后修改时间早于阈值，则删除文件
+        if os.path.isfile(item.path) and file_modified_time < threshold:
+          os.remove(item.path)
+          removed_count +=1
+      except OSError as e:
+        pass
+
+    return removed_count
```

### Comparing `blues_lib-1.0.0/blues_util/BluesImager.py` & `blues_lib-1.0.1/blues_util/BluesImager.py`

 * *Files identical despite different names*

