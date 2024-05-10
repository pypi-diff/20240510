# Comparing `tmp/sqlman-0.2.tar.gz` & `tmp/sqlman-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlman-0.2.tar", last modified: Thu May  9 16:00:25 2024, max compression
+gzip compressed data, was "sqlman-0.3.tar", last modified: Fri May 10 06:05:28 2024, max compression
```

## Comparing `sqlman-0.2.tar` & `sqlman-0.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-09 16:00:25.380459 sqlman-0.2/
--rw-r--r--   0 wangtuo    (501) staff       (20)     3802 2024-05-09 16:00:25.380278 sqlman-0.2/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)     3516 2024-05-09 16:00:14.000000 sqlman-0.2/README.md
--rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-09 16:00:25.380496 sqlman-0.2/setup.cfg
--rw-r--r--   0 wangtuo    (501) staff       (20)      643 2024-05-09 16:00:14.000000 sqlman-0.2/setup.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-09 16:00:25.379314 sqlman-0.2/sqlman/
--rw-r--r--   0 wangtuo    (501) staff       (20)       60 2024-04-17 16:06:46.000000 sqlman-0.2/sqlman/__init__.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     6478 2024-04-21 14:22:23.000000 sqlman-0.2/sqlman/handler.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     9430 2024-04-21 14:32:46.000000 sqlman-0.2/sqlman/table_controller.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     1362 2024-04-21 12:47:57.000000 sqlman-0.2/sqlman/tools.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-09 16:00:25.380117 sqlman-0.2/sqlman.egg-info/
--rw-r--r--   0 wangtuo    (501) staff       (20)     3802 2024-05-09 16:00:25.000000 sqlman-0.2/sqlman.egg-info/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)      276 2024-05-09 16:00:25.000000 sqlman-0.2/sqlman.egg-info/SOURCES.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-09 16:00:25.000000 sqlman-0.2/sqlman.egg-info/dependency_links.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-09 16:00:25.000000 sqlman-0.2/sqlman.egg-info/not-zip-safe
--rw-r--r--   0 wangtuo    (501) staff       (20)       29 2024-05-09 16:00:25.000000 sqlman-0.2/sqlman.egg-info/requires.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        7 2024-05-09 16:00:25.000000 sqlman-0.2/sqlman.egg-info/top_level.txt
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-10 06:05:28.196442 sqlman-0.3/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     4000 2024-05-10 06:05:28.196234 sqlman-0.3/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)     3714 2024-05-10 06:04:43.000000 sqlman-0.3/README.md
+-rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-10 06:05:28.196479 sqlman-0.3/setup.cfg
+-rw-r--r--   0 wangtuo    (501) staff       (20)      643 2024-05-10 05:53:07.000000 sqlman-0.3/setup.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-10 06:05:28.194936 sqlman-0.3/sqlman/
+-rw-r--r--   0 wangtuo    (501) staff       (20)       60 2024-04-17 16:06:46.000000 sqlman-0.3/sqlman/__init__.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     6497 2024-05-10 05:04:46.000000 sqlman-0.3/sqlman/handler.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     9510 2024-05-10 05:43:51.000000 sqlman-0.3/sqlman/table_controller.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1362 2024-04-21 12:47:57.000000 sqlman-0.3/sqlman/tools.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-10 06:05:28.195820 sqlman-0.3/sqlman.egg-info/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     4000 2024-05-10 06:05:28.000000 sqlman-0.3/sqlman.egg-info/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)      292 2024-05-10 06:05:28.000000 sqlman-0.3/sqlman.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-10 06:05:28.000000 sqlman-0.3/sqlman.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-10 06:05:28.000000 sqlman-0.3/sqlman.egg-info/not-zip-safe
+-rw-r--r--   0 wangtuo    (501) staff       (20)       29 2024-05-10 06:05:28.000000 sqlman-0.3/sqlman.egg-info/requires.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        7 2024-05-10 06:05:28.000000 sqlman-0.3/sqlman.egg-info/top_level.txt
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-10 06:05:28.195929 sqlman-0.3/tests/
+-rw-r--r--   0 wangtuo    (501) staff       (20)      279 2024-05-10 05:38:51.000000 sqlman-0.3/tests/test-0.py
```

### Comparing `sqlman-0.2/PKG-INFO` & `sqlman-0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-Metadata-Version: 2.1
-Name: sqlman
-Version: 0.2
-Summary: 告别SQL语句，python操作mysql的贴心助手
-Home-page: https://github.com/markadc/sqlman
-Author: WangTuo
-Author-email: markadc@126.com
-License: MIT
-Keywords: Python,MySQL,Database
-Description-Content-Type: text/markdown
+# 如何安装？
 
-# 如何吸引你？
+- `pip install sqlman`
 
-### 如此简易的连接方式
+---
 
-一个字典参数即可
+# 拿什么吸引你这个靓仔？
 
-### 插入数据如此的贴心
+- 使用方式简单暴力
 
-自动推导
+- 不用写SQL就能进行增删改查
 
-- 传入dict是插入一条数据，传入list是插入多条数据
+---
 
-插入模式
+### 连接方式是如此简易
 
-- 默认插入，数据冲突则报错
-- 插入时，数据冲突则不报错
-- 插入时，数据冲突则不报错，还可以同时更新数据
-- 插入时，则提前过滤掉会冲突的数据，只插入不冲突的数据
+- 一个字典参数即可
+
+---
+
+### 插入数据是如此贴心
+
+- 自动推导
+    - 传入dict是插入一条数据，传入list是插入多条数据
+
+- 多种插入模式
+    - 模式1，插入时，数据冲突则报错
+    - 模式2，插入时，数据冲突则忽略
+    - 模式3，插入时，数据发生冲突，把数据进行更新操作
+    - 模式4，插入时，自动过滤掉冲突的数据，只插入不冲突的数据
 
 ### 等等等等...
 
-# 具体演示
+---
+
+# 操练起来
 
 ### 连接mysql
 
 ```python
 from sqlman import Handler
 
 # 用来连接test数据库
@@ -158,8 +161,8 @@
 people.scan()
 
 # 限制id范围为101~222，每轮扫描100条，每轮的回调函数为show
 people.scan('people', sort_field='id', start=101, end=222, once=100, dealer=show)
 
 # 限制id范围的基础上，限制age=18
 people.scan('people', sort_field='id', start=101, end=222, once=100, dealer=show, add_cond='age=18')
-```
+```
```

### Comparing `sqlman-0.2/README.md` & `sqlman-0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,54 @@
-# 如何吸引你？
+Metadata-Version: 2.1
+Name: sqlman
+Version: 0.3
+Summary: 告别SQL语句，python操作mysql的贴心助手
+Home-page: https://github.com/markadc/sqlman
+Author: WangTuo
+Author-email: markadc@126.com
+License: MIT
+Keywords: Python,MySQL,Database
+Description-Content-Type: text/markdown
 
-### 如此简易的连接方式
+# 如何安装？
 
-一个字典参数即可
+- `pip install sqlman`
 
-### 插入数据如此的贴心
+---
 
-自动推导
+# 拿什么吸引你这个靓仔？
 
-- 传入dict是插入一条数据，传入list是插入多条数据
+- 使用方式简单暴力
 
-插入模式
+- 不用写SQL就能进行增删改查
 
-- 默认插入，数据冲突则报错
-- 插入时，数据冲突则不报错
-- 插入时，数据冲突则不报错，还可以同时更新数据
-- 插入时，则提前过滤掉会冲突的数据，只插入不冲突的数据
+---
+
+### 连接方式是如此简易
+
+- 一个字典参数即可
+
+---
+
+### 插入数据是如此贴心
+
+- 自动推导
+    - 传入dict是插入一条数据，传入list是插入多条数据
+
+- 多种插入模式
+    - 模式1，插入时，数据冲突则报错
+    - 模式2，插入时，数据冲突则忽略
+    - 模式3，插入时，数据发生冲突，把数据进行更新操作
+    - 模式4，插入时，自动过滤掉冲突的数据，只插入不冲突的数据
 
 ### 等等等等...
 
-# 具体演示
+---
+
+# 操练起来
 
 ### 连接mysql
 
 ```python
 from sqlman import Handler
 
 # 用来连接test数据库
@@ -147,8 +172,8 @@
 people.scan()
 
 # 限制id范围为101~222，每轮扫描100条，每轮的回调函数为show
 people.scan('people', sort_field='id', start=101, end=222, once=100, dealer=show)
 
 # 限制id范围的基础上，限制age=18
 people.scan('people', sort_field='id', start=101, end=222, once=100, dealer=show, add_cond='age=18')
-```
+```
```

### Comparing `sqlman-0.2/setup.py` & `sqlman-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='sqlman',
-    version='0.2',
+    version='0.3',
     description='告别SQL语句，python操作mysql的贴心助手',
     url='https://github.com/markadc/sqlman',
     author='WangTuo',
     author_email='markadc@126.com',
     packages=find_packages(),
     license='MIT',
     zip_safe=False,
```

### Comparing `sqlman-0.2/sqlman/handler.py` & `sqlman-0.3/sqlman/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,39 +54,41 @@
     def exe_sql(self, sql: str, args=None, mode=0, dict_cursor=True) -> dict:
         """执行SQL"""
         cur, con = None, None
         try:
             cur, con = self.open_connect(dict_cursor)
             line = cur.execute(sql, args=args)
             con.commit()
+            query_results = None if mode == 0 else list(cur.fetchall()) if mode > 1 else cur.fetchone()
+            return build_result(status=1, affect=line, query=query_results)
+
         except Exception as e:
             self.panic(sql, e)
             if con:
                 con.rollback()
-            return build_result(status=0)
-        else:
-            data = None if not mode else list(cur.fetchall()) if mode > 1 else cur.fetchone()
-            return build_result(status=1, affect=line, query=data)
+            return build_result(status=0, error=str(e))
+
         finally:
             self.close_connect(cur, con)
 
     def exem_sql(self, sql: str, args=None) -> int:
         """批量执行SQL"""
         cur, con = None, None
         try:
             cur, con = self.open_connect()
             line = cur.executemany(sql, args=args)
             con.commit()
+            return line
+
         except Exception as e:
             self.panic(sql, e)
             if con:
                 con.rollback()
             return 0
-        else:
-            return line
+
         finally:
             self.close_connect(cur, con)
 
     def _insert_one(self, table: str, item: dict, update: str = None, unique_index: str = None) -> int:
         """
         插入数据
         Args:
@@ -100,16 +102,16 @@
         """
         fields = ', '.join(item.keys())
         values = ', '.join(['%s'] * len(item.keys()))
         new = '' if not (update or unique_index) else 'ON DUPLICATE KEY UPDATE {}'.format(
             update or '{}={}'.format(unique_index, unique_index)
         )
         sql = 'insert into {}({}) value({}) {}'.format(table, fields, values, new)
-        res = self.exe_sql(sql, args=tuple(item.values()))['affect']
-        return res
+        affect = self.exe_sql(sql, args=tuple(item.values()))['affect']
+        return affect
 
     def _insert_many(self, table: str, items: list, update: str = None, unique_index: str = None) -> int:
         """
         批量插入数据
         Args:
             table: 表
             items: 数据
@@ -121,16 +123,16 @@
         """
         fields = ', '.join(items[0].keys())
         values = ', '.join(['%s'] * len(items[0].keys()))
         new = '' if not (update or unique_index) else 'ON DUPLICATE KEY UPDATE {}'.format(
             update or '{}={}'.format(unique_index, unique_index)
         )
         sql = 'insert into {}({}) value({}) {}'.format(table, fields, values, new)
-        line = self.exem_sql(sql, args=[tuple(item.values()) for item in items])
-        return line
+        affect = self.exem_sql(sql, args=[tuple(item.values()) for item in items])
+        return affect
 
     def make_datas(self, table: str, once=1000, total=10000):
         """新增测试表并添加测试数据"""
         import random
         from faker import Faker
 
         faker = Faker("zh_cn")
```

### Comparing `sqlman-0.2/sqlman/table_controller.py` & `sqlman-0.3/sqlman/table_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -234,16 +234,24 @@
             times += 1
             if max_query_times and times >= max_query_times:  # 达到最大查询次数了
                 break
 
             first_query = False
             time.sleep(rest)  # 每一轮查询之间的间隔
 
-    def insert_data(self, data: dict | list | tuple, update: str = None, unique_index: str = None) -> int:
-        """批量插入数据"""
+    def insert_data(self, data: dict | list, update: str = None, unique_index: str = None) -> int:
+        """
+        插入数据，dict插入一条，list插入多条
+        Args:
+            data: {} | [{}, {}, {}]
+
+        Returns:
+            已插入的行数
+
+        """
         if isinstance(data, dict):
             return super()._insert_one(self.table, data, update, unique_index)
         return super()._insert_many(self.table, list(data), update, unique_index)
 
     def check_values(self, field: str, values: list) -> tuple:
         """
         检查字段的多个值
@@ -257,20 +265,19 @@
         data = self.query(pick=field, **{field: values})
         old = [one[field] for one in data]
         new = list(set(values) - set(old))
         return new, old
 
     def dedup_insert_data(self, items: list, dedup_field: str) -> int:
         """
-        批量插入数据\n
-        如果数据跟数据库中重复，则自动过滤掉
+        去重版插入数据
         Args:
-            items: 这些数据
-            dedup_field: 需要去重的字段
+            items: [{}, {}, {}]
+            dedup_field: 进行去重的字段
 
         Returns:
-            受影响的行数
+            已插入的行数
         """
         to_check = [this[dedup_field] for this in items]
         new_values = self.check_values(dedup_field, to_check)[0]
         new_items = [this for this in items if this[dedup_field] in new_values]
         return self.insert_data(new_items, unique_index=dedup_field) if new_items else 0
```

### Comparing `sqlman-0.2/sqlman/tools.py` & `sqlman-0.3/sqlman/tools.py`

 * *Files identical despite different names*

### Comparing `sqlman-0.2/sqlman.egg-info/PKG-INFO` & `sqlman-0.3/sqlman.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,54 @@
 Metadata-Version: 2.1
 Name: sqlman
-Version: 0.2
+Version: 0.3
 Summary: 告别SQL语句，python操作mysql的贴心助手
 Home-page: https://github.com/markadc/sqlman
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
 Keywords: Python,MySQL,Database
 Description-Content-Type: text/markdown
 
-# 如何吸引你？
+# 如何安装？
 
-### 如此简易的连接方式
+- `pip install sqlman`
 
-一个字典参数即可
+---
 
-### 插入数据如此的贴心
+# 拿什么吸引你这个靓仔？
 
-自动推导
+- 使用方式简单暴力
 
-- 传入dict是插入一条数据，传入list是插入多条数据
+- 不用写SQL就能进行增删改查
 
-插入模式
+---
 
-- 默认插入，数据冲突则报错
-- 插入时，数据冲突则不报错
-- 插入时，数据冲突则不报错，还可以同时更新数据
-- 插入时，则提前过滤掉会冲突的数据，只插入不冲突的数据
+### 连接方式是如此简易
+
+- 一个字典参数即可
+
+---
+
+### 插入数据是如此贴心
+
+- 自动推导
+    - 传入dict是插入一条数据，传入list是插入多条数据
+
+- 多种插入模式
+    - 模式1，插入时，数据冲突则报错
+    - 模式2，插入时，数据冲突则忽略
+    - 模式3，插入时，数据发生冲突，把数据进行更新操作
+    - 模式4，插入时，自动过滤掉冲突的数据，只插入不冲突的数据
 
 ### 等等等等...
 
-# 具体演示
+---
+
+# 操练起来
 
 ### 连接mysql
 
 ```python
 from sqlman import Handler
 
 # 用来连接test数据库
```

