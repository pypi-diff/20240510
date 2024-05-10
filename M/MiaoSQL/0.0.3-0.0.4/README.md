# Comparing `tmp/MiaoSQL-0.0.3.tar.gz` & `tmp/MiaoSQL-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MiaoSQL-0.0.3.tar", last modified: Tue May  7 04:53:46 2024, max compression
+gzip compressed data, was "MiaoSQL-0.0.4.tar", last modified: Fri May 10 14:33:58 2024, max compression
```

## Comparing `MiaoSQL-0.0.3.tar` & `MiaoSQL-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 04:53:46.721742 MiaoSQL-0.0.3/
-drwxrwxrwx   0        0        0        0 2024-05-07 04:53:46.717229 MiaoSQL-0.0.3/MiaoSQL/
--rw-rw-rw-   0        0        0        0 2024-03-18 14:02:58.000000 MiaoSQL-0.0.3/MiaoSQL/__init__.py
--rw-rw-rw-   0        0        0     9460 2024-05-07 04:49:25.000000 MiaoSQL-0.0.3/MiaoSQL/miaosql.py
-drwxrwxrwx   0        0        0        0 2024-05-07 04:53:46.720228 MiaoSQL-0.0.3/MiaoSQL.egg-info/
--rw-rw-rw-   0        0        0      300 2024-05-07 04:53:46.000000 MiaoSQL-0.0.3/MiaoSQL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2024-05-07 04:53:46.000000 MiaoSQL-0.0.3/MiaoSQL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 04:53:46.000000 MiaoSQL-0.0.3/MiaoSQL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-07 04:53:46.000000 MiaoSQL-0.0.3/MiaoSQL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      300 2024-05-07 04:53:46.721742 MiaoSQL-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-07 04:53:46.721742 MiaoSQL-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      420 2024-05-07 04:53:40.000000 MiaoSQL-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:33:58.743469 MiaoSQL-0.0.4/
+drwxrwxrwx   0        0        0        0 2024-05-10 14:33:58.738852 MiaoSQL-0.0.4/MiaoSQL/
+-rw-rw-rw-   0        0        0       37 2024-05-10 05:25:21.000000 MiaoSQL-0.0.4/MiaoSQL/Exception.py
+-rw-rw-rw-   0        0        0        0 2024-03-18 14:02:58.000000 MiaoSQL-0.0.4/MiaoSQL/__init__.py
+-rw-rw-rw-   0        0        0     9706 2024-05-10 14:05:37.000000 MiaoSQL-0.0.4/MiaoSQL/miaosql.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:33:58.741854 MiaoSQL-0.0.4/MiaoSQL.egg-info/
+-rw-rw-rw-   0        0        0      300 2024-05-10 14:33:58.000000 MiaoSQL-0.0.4/MiaoSQL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-05-10 14:33:58.000000 MiaoSQL-0.0.4/MiaoSQL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 14:33:58.000000 MiaoSQL-0.0.4/MiaoSQL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-10 14:33:58.000000 MiaoSQL-0.0.4/MiaoSQL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      300 2024-05-10 14:33:58.741854 MiaoSQL-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-10 14:33:58.743469 MiaoSQL-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      420 2024-05-10 14:33:44.000000 MiaoSQL-0.0.4/setup.py
```

### Comparing `MiaoSQL-0.0.3/MiaoSQL/miaosql.py` & `MiaoSQL-0.0.4/MiaoSQL/miaosql.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,17 @@
             database: 数据库名
         }
     """
 
     cursor = None
     _sjk = None
 
+    raw_data = None
+    _out_cols = None
+
     # 数据库连接
     def __init__(self, con: dict):
         """初始化数据库对象"""
         self._config = con
         self._sjk = pymysql.connect(**self._config)
         self.cursor = self._sjk.cursor()
 
@@ -323,14 +326,24 @@
         if type(s) == str:
             s = emoji.demojize(s, delimiters=(" ", " "))
             s = s.replace(r"\"", '"').replace("\\", "").replace('"', r"\"")
             return '"' + s + '"'
         else:
             return str(s)
 
+    def get_DictInList(self):
+        res = self.cursor.fetchall()
+        pass
+
+    def ping(self):
+        self._sjk.ping(reconnect=True)
+
+    def commit(self):
+        self._sjk.commit()
+
 
 # OpenMySql的with版本
 class OpenMiaoSql:
     """MySql的with版本"""
 
     sql = None
```

