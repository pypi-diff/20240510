# Comparing `tmp/xtn-tools-pro-1.0.0.0.3.tar.gz` & `tmp/xtn-tools-pro-1.0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtn-tools-pro-1.0.0.0.3.tar", last modified: Sat Apr 27 07:51:03 2024, max compression
+gzip compressed data, was "dist\xtn-tools-pro-1.0.0.0.4.tar", last modified: Fri May 10 00:04:47 2024, max compression
```

## Comparing `xtn-tools-pro-1.0.0.0.3.tar` & `xtn-tools-pro-1.0.0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtn-tools-pro-1.0.0.0.3/LICENSE
--rw-rw-rw-   0        0        0      287 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtn-tools-pro-1.0.0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1210 2024-04-27 06:01:26.000000 xtn-tools-pro-1.0.0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/
--rw-rw-rw-   0        0        0      395 2024-04-18 05:24:09.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/db/
--rw-rw-rw-   0        0        0     5567 2024-04-19 08:42:19.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/db/MongoDB.py
--rw-rw-rw-   0        0        0     6053 2024-04-27 07:30:36.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/db/RedisDB.py
--rw-rw-rw-   0        0        0      416 2024-04-18 05:40:27.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/proxy/
--rw-rw-rw-   0        0        0     9842 2024-04-27 07:38:44.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/proxy/XiaoXiangProxy.py
--rw-rw-rw-   0        0        0      418 2024-04-27 04:18:50.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/proxy/__init__.py
--rw-rw-rw-   0        0        0     2630 2024-04-19 10:12:45.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/tools.py
--rw-rw-rw-   0        0        0     1512 2024-04-19 10:21:05.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/tools_flie.py
--rw-rw-rw-   0        0        0     4867 2024-04-19 10:12:45.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/tools_time.py
-drwxrwxrwx   0        0        0        0 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro.egg-info/
--rw-rw-rw-   0        0        0      287 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtn-tools-pro-1.0.0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      287 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtn-tools-pro-1.0.0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2024-05-10 00:03:27.000000 xtn-tools-pro-1.0.0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/
+-rw-rw-rw-   0        0        0      395 2024-04-18 05:24:09.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/db/
+-rw-rw-rw-   0        0        0     5567 2024-04-19 08:42:19.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/db/MongoDB.py
+-rw-rw-rw-   0        0        0     6053 2024-04-27 07:30:36.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/db/RedisDB.py
+-rw-rw-rw-   0        0        0      416 2024-04-18 05:40:27.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/proxy/
+-rw-rw-rw-   0        0        0     9842 2024-04-27 07:38:44.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/proxy/XiaoXiangProxy.py
+-rw-rw-rw-   0        0        0      418 2024-04-27 04:18:50.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/proxy/__init__.py
+-rw-rw-rw-   0        0        0     3502 2024-05-10 00:00:28.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/tools.py
+-rw-rw-rw-   0        0        0     1512 2024-04-19 10:21:05.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/tools_flie.py
+-rw-rw-rw-   0        0        0     4867 2024-04-19 10:12:45.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/tools_time.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-10 00:04:47.000000 xtn-tools-pro-1.0.0.0.4/xtn_tools_pro.egg-info/top_level.txt
```

### Comparing `xtn-tools-pro-1.0.0.0.3/setup.py` & `xtn-tools-pro-1.0.0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="xtn-tools-pro",  # 模块名称
-    version="1.0.0.0.3",  # 版本
+    version="1.0.0.0.4",  # 版本
     author="xtn",  # 作者
     author_email="czw011122@163.com",  # 作者邮箱
     description="xtn 开发工具",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据(更多描述信息)
```

### Comparing `xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/db/MongoDB.py` & `xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/db/MongoDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/db/RedisDB.py` & `xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/db/RedisDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/proxy/XiaoXiangProxy.py` & `xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/proxy/XiaoXiangProxy.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/tools.py` & `xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/tools.py`

 * *Files 27% similar despite different names*

```diff
@@ -33,33 +33,62 @@
     :param is_upper: 是否转大写 默认False
     :return:
     """
     result = get_md5_32(s, is_upper)
     return result[8:24]
 
 
-def get_file_md5_32(file_path):
+def get_binary_content_md5_32(content, is_upper=False):
+    """
+        二进制内容md5 例如图片
+    :param content: 二进制内容
+    :param is_upper: 是否转大写 默认False
+    :return:
+    """
+    md5_hash = hashlib.md5(content)
+    md5_hexdigest = md5_hash.hexdigest()
+    if is_upper:
+        return md5_hexdigest.upper()
+    return md5_hexdigest
+
+
+def get_binary_content_md5_16(content, is_upper=False):
+    """
+        二进制内容md5 例如图片
+    :param content: 二进制内容
+    :param is_upper: 是否转大写 默认False
+    :return:
+    """
+    result = get_binary_content_md5_32(content, is_upper)
+    return result[8:24]
+
+
+def get_file_md5_32(file_path, is_upper=False):
     """
         获取文件md5值
     :param file_path: 文件路径
+    :param is_upper: 是否转大写 默认False
     :return: 
     """
     with open(file_path, 'rb') as file:
         data = file.read()
         md5_hash = hashlib.md5(data).hexdigest()
+    if is_upper:
+        return md5_hash.upper()
     return md5_hash
 
 
-def get_file_md5_16(file_path):
+def get_file_md5_16(file_path, is_upper=False):
     """
         获取文件md5值
     :param file_path: 文件路径
+    :param is_upper: 是否转大写 默认False
     :return: 
     """
-    result = get_file_md5_32(file_path)
+    result = get_file_md5_32(file_path, is_upper)
     return result[8:24]
 
 
 def get_str_to_json(str_json):
     """
         字符串类型的json格式 转 json
     :param str_json: 字符串json
@@ -96,13 +125,9 @@
     if limit <= 0:
         return 0
     # 根据总条数和limit计算总页数
     total_pages = math.ceil(total / limit)
     return total_pages
 
 
-
-
-
-
 if __name__ == '__main__':
     pass
```

### Comparing `xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/tools_flie.py` & `xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/tools_flie.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/tools_time.py` & `xtn-tools-pro-1.0.0.0.4/xtn_tools_pro/tools_time.py`

 * *Files identical despite different names*

