# Comparing `tmp/middleware-help-python-0.0.7.tar.gz` & `tmp/middleware-help-python-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "middleware-help-python-0.0.7.tar", last modified: Mon May  6 15:19:58 2024, max compression
+gzip compressed data, was "middleware-help-python-0.0.8.tar", last modified: Fri May 10 10:36:05 2024, max compression
```

## Comparing `middleware-help-python-0.0.7.tar` & `middleware-help-python-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 15:19:58.692155 middleware-help-python-0.0.7/
--rw-rw-rw-   0        0        0    11558 2024-04-24 07:47:20.000000 middleware-help-python-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      543 2024-05-06 15:19:58.691158 middleware-help-python-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       24 2024-04-24 07:47:20.000000 middleware-help-python-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 15:19:58.689164 middleware-help-python-0.0.7/middleware_help_python.egg-info/
--rw-rw-rw-   0        0        0      543 2024-05-06 15:19:58.000000 middleware-help-python-0.0.7/middleware_help_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2024-05-06 15:19:58.000000 middleware-help-python-0.0.7/middleware_help_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 15:19:58.000000 middleware-help-python-0.0.7/middleware_help_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-06 15:19:58.000000 middleware-help-python-0.0.7/middleware_help_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-06 15:19:58.000000 middleware-help-python-0.0.7/middleware_help_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 15:19:58.686196 middleware-help-python-0.0.7/middleware_helper/
--rw-rw-rw-   0        0        0      480 2024-04-24 07:50:59.000000 middleware-help-python-0.0.7/middleware_helper/__init__.py
--rw-rw-rw-   0        0        0     3878 2024-05-06 15:13:25.000000 middleware-help-python-0.0.7/middleware_helper/mysql.py
--rw-rw-rw-   0        0        0     2155 2024-04-29 08:20:12.000000 middleware-help-python-0.0.7/middleware_helper/network.py
--rw-rw-rw-   0        0        0     1267 2024-04-29 08:21:12.000000 middleware-help-python-0.0.7/middleware_helper/redis.py
--rw-rw-rw-   0        0        0       42 2024-05-06 15:19:58.692155 middleware-help-python-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1162 2024-05-06 15:12:36.000000 middleware-help-python-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 10:36:05.471533 middleware-help-python-0.0.8/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 07:47:20.000000 middleware-help-python-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      543 2024-05-10 10:36:05.469564 middleware-help-python-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2024-04-24 07:47:20.000000 middleware-help-python-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 10:36:05.468564 middleware-help-python-0.0.8/middleware_help_python.egg-info/
+-rw-rw-rw-   0        0        0      543 2024-05-10 10:36:05.000000 middleware-help-python-0.0.8/middleware_help_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-05-10 10:36:05.000000 middleware-help-python-0.0.8/middleware_help_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 10:36:05.000000 middleware-help-python-0.0.8/middleware_help_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-10 10:36:05.000000 middleware-help-python-0.0.8/middleware_help_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-10 10:36:05.000000 middleware-help-python-0.0.8/middleware_help_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 10:36:05.465572 middleware-help-python-0.0.8/middleware_helper/
+-rw-rw-rw-   0        0        0      480 2024-04-24 07:50:59.000000 middleware-help-python-0.0.8/middleware_helper/__init__.py
+-rw-rw-rw-   0        0        0      530 2024-05-10 10:22:25.000000 middleware-help-python-0.0.8/middleware_helper/libs.py
+-rw-rw-rw-   0        0        0     5026 2024-05-10 10:35:38.000000 middleware-help-python-0.0.8/middleware_helper/mysql.py
+-rw-rw-rw-   0        0        0     2155 2024-04-29 08:20:12.000000 middleware-help-python-0.0.8/middleware_helper/network.py
+-rw-rw-rw-   0        0        0     1267 2024-04-29 08:21:12.000000 middleware-help-python-0.0.8/middleware_helper/redis.py
+-rw-rw-rw-   0        0        0       42 2024-05-10 10:36:05.472554 middleware-help-python-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2024-05-10 10:35:53.000000 middleware-help-python-0.0.8/setup.py
```

### Comparing `middleware-help-python-0.0.7/LICENSE` & `middleware-help-python-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.0.7/PKG-INFO` & `middleware-help-python-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: middleware-help-python
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is my middleware help package
 Home-page: https://github.com/ckf10000/middleware-help-python
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `middleware-help-python-0.0.7/middleware_help_python.egg-info/PKG-INFO` & `middleware-help-python-0.0.8/middleware_help_python.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: middleware-help-python
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is my middleware help package
 Home-page: https://github.com/ckf10000/middleware-help-python
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `middleware-help-python-0.0.7/middleware_helper/mysql.py` & `middleware-help-python-0.0.8/middleware_helper/mysql.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,32 +6,62 @@
 # Description:  TODO
 # Author:       mfkifhss2023
 # CreateDate:   2024/04/24
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from mysql.connector import connect
+from middleware_helper.libs import logger
 from mysql.connector.cursor_cext import CMySQLCursor
 from middleware_helper.network import filter_system_port_list
 
 
 class Mysql(object):
 
     def __init__(self, **mysql_params_map):
-        port = mysql_params_map.get("port")
-        if isinstance(port, list):
-            mysql_params_map["port"] = filter_system_port_list(data_port=port, default_port=3306)
-        self.conn = connect(
-            host=mysql_params_map.get("host"),
-            user=mysql_params_map.get("user"),
-            port=mysql_params_map.get("port"),
-            charset=mysql_params_map.get("charset"),
-            password=mysql_params_map.get("password"),
-            database=mysql_params_map.get("database")
-        )
+        self.host = mysql_params_map.get('host') or '127.0.0.1'
+        self.port = mysql_params_map.get("port") or '3306'
+        self.user = mysql_params_map.get("user") or 'root'
+        self.password = mysql_params_map.get("password") or 'Admin@123'
+        self.database = mysql_params_map.get("database") or 'mysql'
+        self.charset = mysql_params_map.get("charset") or 'utf8'
+        self.conn = self.retry_connection()
+
+    def __connect_to_mysql(self) -> connect:
+        try:
+            if isinstance(self.port, list):
+                __port = filter_system_port_list(data_port=self.port, default_port=3306)
+            else:
+                __port = self.port
+            # 建立连接
+            conn = connect(
+                host=self.host,
+                user=self.user,
+                port=__port,
+                charset=self.charset,
+                password=self.password,
+                database=self.database
+            )
+            return conn
+        except Exception as e:
+            logger.error("数据库连接失败: {}".format(e))
+            return None
+
+    def retry_connection(self) -> connect:
+        conn = self.__connect_to_mysql()
+        i = 0
+        while conn is None or not conn.is_connected():
+            if i > 9:
+                logger.warning("尝试连接数据库10次以上，最终未能成功")
+            else:
+                if i > 0:
+                    logger.warning("尝试重连数据库...")
+                conn = self.__connect_to_mysql()
+            i = i + 1
+        return conn
 
     @classmethod
     def convert_tuple_to_dict(cls, records: list, column_names: tuple) -> list:
         # 将元组列表转换为字典列表
         result_list = []
         for row in records:
             row_dict = {}
@@ -50,35 +80,35 @@
         # 获取列名
         column_names = cursor.column_names
         result_list = cls.convert_tuple_to_dict(records=records, column_names=column_names)
         return result_list
 
     def execute_sql(self, sql: str, action: str):
         results = None
-        if self.conn.is_connected():
+        if self.conn and self.conn.is_connected():
             cursor: CMySQLCursor = self.conn.cursor()
             if action in ("insert", "update", "delete"):
                 try:
                     cursor.execute(sql)
                     self.conn.commit()
                 except Exception as e:
-                    print(e)
+                    logger.error(e)
                     self.conn.rollback()
             elif action == "select":
                 try:
                     # 获取查询结果
                     results = self.cursor_query_data(sql=sql, cursor=cursor)
                 except Exception as e:
-                    print(e)
+                    logger.error(e)
             else:
                 pass
             cursor.close()
             self.conn.close()
         else:
-            print("当前连接不正常.")
+            logger.error("当前连接不正常.")
         return results
 
     @classmethod
     def convert_key_value_str(cls, **kwargs) -> tuple:
         field_list, value_list = list(), list()
         for key, value in kwargs.items():
             if value is None:
```

### Comparing `middleware-help-python-0.0.7/middleware_helper/network.py` & `middleware-help-python-0.0.8/middleware_helper/network.py`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.0.7/middleware_helper/redis.py` & `middleware-help-python-0.0.8/middleware_helper/redis.py`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.0.7/setup.py` & `middleware-help-python-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='middleware-help-python',
-    version='0.0.7',
+    version='0.0.8',
     description='This is my middleware help package',
     long_description='This is my middleware help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/middleware-help-python',
     packages=find_packages(),
     install_requires=[
```

