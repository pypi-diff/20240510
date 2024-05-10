# Comparing `tmp/doupand-1.0.3.tar.gz` & `tmp/doupand-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/doupand-1.0.3.tar", last modified: Tue Apr 11 13:57:19 2023, max compression
+gzip compressed data, was "doupand-1.0.9.tar", last modified: Fri May  3 14:52:49 2024, max compression
```

## Comparing `doupand-1.0.3.tar` & `doupand-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-11 13:57:19.000000 doupand-1.0.3/
--rw-r--r--   0 tongjun    (501) staff       (20)     2041 2023-04-11 13:57:19.000000 doupand-1.0.3/PKG-INFO
--rw-r--r--   0 tongjun    (501) staff       (20)     1469 2023-04-07 19:08:40.000000 doupand-1.0.3/LICENSE
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand/
--rw-r--r--   0 tongjun    (501) staff       (20)      133 2023-04-08 17:33:37.000000 doupand-1.0.3/doupand/__init__.py
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand/utils/
--rw-r--r--   0 tongjun    (501) staff       (20)      701 2023-04-07 14:51:56.000000 doupand-1.0.3/doupand/utils/userauth.py
--rw-r--r--   0 tongjun    (501) staff       (20)        0 2023-04-06 17:18:45.000000 doupand-1.0.3/doupand/utils/__init__.py
--rw-r--r--   0 tongjun    (501) staff       (20)      277 2023-04-08 17:11:54.000000 doupand-1.0.3/doupand/utils/cons.py
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand/api/
--rw-r--r--   0 tongjun    (501) staff       (20)     3183 2023-04-11 13:54:16.000000 doupand-1.0.3/doupand/api/client.py
--rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-06 17:31:40.000000 doupand-1.0.3/doupand/api/__init__.py
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/
--rw-r--r--   0 tongjun    (501) staff       (20)     2041 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/PKG-INFO
--rw-r--r--   0 tongjun    (501) staff       (20)      310 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/SOURCES.txt
--rw-r--r--   0 tongjun    (501) staff       (20)       16 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/requires.txt
--rw-r--r--   0 tongjun    (501) staff       (20)        8 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/top_level.txt
--rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/dependency_links.txt
--rw-r--r--   0 tongjun    (501) staff       (20)     2400 2023-04-11 13:39:22.000000 doupand-1.0.3/setup.py
--rw-r--r--   0 tongjun    (501) staff       (20)       38 2023-04-11 13:57:19.000000 doupand-1.0.3/setup.cfg
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-05-03 14:52:49.518100 doupand-1.0.9/
+-rw-r--r--   0 tongjun    (501) staff       (20)     1469 2023-04-07 19:08:40.000000 doupand-1.0.9/LICENSE
+-rw-r--r--   0 tongjun    (501) staff       (20)     2039 2024-05-03 14:52:49.517936 doupand-1.0.9/PKG-INFO
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-05-03 14:52:49.515765 doupand-1.0.9/doupand/
+-rw-r--r--   0 tongjun    (501) staff       (20)      134 2024-05-03 14:50:41.000000 doupand-1.0.9/doupand/__init__.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-05-03 14:52:49.517085 doupand-1.0.9/doupand/api/
+-rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-06 17:31:40.000000 doupand-1.0.9/doupand/api/__init__.py
+-rw-r--r--   0 tongjun    (501) staff       (20)     3362 2024-05-03 14:50:41.000000 doupand-1.0.9/doupand/api/client.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-05-03 14:52:49.517603 doupand-1.0.9/doupand/utils/
+-rw-r--r--   0 tongjun    (501) staff       (20)        0 2023-04-06 17:18:45.000000 doupand-1.0.9/doupand/utils/__init__.py
+-rw-r--r--   0 tongjun    (501) staff       (20)      277 2023-04-08 17:11:54.000000 doupand-1.0.9/doupand/utils/cons.py
+-rw-r--r--   0 tongjun    (501) staff       (20)      701 2024-04-26 14:54:25.000000 doupand-1.0.9/doupand/utils/userauth.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-05-03 14:52:49.516677 doupand-1.0.9/doupand.egg-info/
+-rw-r--r--   0 tongjun    (501) staff       (20)     2039 2024-05-03 14:52:49.000000 doupand-1.0.9/doupand.egg-info/PKG-INFO
+-rw-r--r--   0 tongjun    (501) staff       (20)      310 2024-05-03 14:52:49.000000 doupand-1.0.9/doupand.egg-info/SOURCES.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)        1 2024-05-03 14:52:49.000000 doupand-1.0.9/doupand.egg-info/dependency_links.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)       16 2024-05-03 14:52:49.000000 doupand-1.0.9/doupand.egg-info/requires.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)        8 2024-05-03 14:52:49.000000 doupand-1.0.9/doupand.egg-info/top_level.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)       38 2024-05-03 14:52:49.518152 doupand-1.0.9/setup.cfg
+-rw-r--r--   0 tongjun    (501) staff       (20)     2400 2024-05-03 14:52:30.000000 doupand-1.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `doupand-1.0.3/PKG-INFO` & `doupand-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doupand
-Version: 1.0.3
+Version: 1.0.9
 Summary: A simple and easy-to-use financial data interface library built for normal investors!
 Home-page: https://doupand.com
 Author: DouBro
 Author-email: doupand@163.com
 License: BSD
 Keywords: Financial Data Interface
 Platform: all
@@ -62,9 +62,7 @@
     4     000005.SZ  000005  ...         SZSE          主板
     ...         ...     ...  ...          ...         ...
     5329  873169.BJ  873169  ...          BSE         北交所
     5330  873223.BJ  873223  ...          BSE         北交所
     5331  873305.BJ  873305  ...          BSE         北交所
     5332  873339.BJ  873339  ...          BSE         北交所
     5333  873527.BJ  873527  ...          BSE         北交所
-
-
```

### Comparing `doupand-1.0.3/LICENSE` & `doupand-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `doupand-1.0.3/doupand/utils/userauth.py` & `doupand-1.0.9/doupand/utils/userauth.py`

 * *Files identical despite different names*

### Comparing `doupand-1.0.3/doupand/api/client.py` & `doupand-1.0.9/doupand/api/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # -*-coding: utf-8 -*-
 # @Time    : 2023/4/7 01:32
 # @Description  : API数据接口
 
 import json
 import os
+
+import ipdb
 import requests
 import time
 import pandas as pd
 from functools import partial
 from doupand.utils import userauth
 from doupand.utils import cons as ct
 
-__all__ = ['datareader']
+__all__ = ['data_reader']
 
 
 class DataReader:
     __token = ''
     __http_url = ''
     __distribution_url = 'http://api.doupand.com'
 
@@ -32,15 +34,15 @@
     def __query_token(self):
         """请求口令token"""
         if self.__token == '' or self.__token is None:
             token = userauth.get_token()
             if token is not None and token != '':
                 self.__token = token
             else:
-                raise Exception('DataReader Init Error!')
+                raise Exception('DataReader初始化失败，未设置TOKEN!')
 
         return self.__token
 
     @property
     def __query_url(self):
         """请求URL"""
         cur_time = int(time.time())
@@ -52,41 +54,42 @@
 
             if os.path.exists(fp):
                 df = pd.read_csv(fp)
                 if cur_time < int(df.loc[0]['expire_time']):
                     self.__url_expire_time = int(df.loc[0]['expire_time'])
                     return str(df.loc[0]['http_url'])
 
-            res = requests.post(self.__distribution_url, timeout=10, headers={'Connection': 'close'})
+            req_params = {'token': self.__query_token}
+            res = requests.post(self.__distribution_url, json=req_params, timeout=10, headers={'Connection': 'close'})
             result = res.json()
             if result['status'] == "success":
-                self.__http_url = res.json()['result']
-                self.__url_expire_time = cur_time + 12 * 60 * 60
+                self.__http_url = result['result']
+                valid_period = result['valid_period']
+                self.__url_expire_time = cur_time + valid_period
                 df = pd.DataFrame([[self.__http_url, self.__url_expire_time]], columns=['http_url', 'expire_time'])
                 df.to_csv(fp, index=False)
                 return self.__http_url
             else:
                 raise Exception("初始化请求失败，请重试！")
 
-    def query(self, api_name, fields='', **kwargs):
+    def query(self, api_name, **kwargs):
         """
         请求API
         :param api_name: API名称
         :param fields: 返回字段
         :param kwargs: 参数
         :return:
         """
         req_params = {
             'api_name': api_name,
             'token': self.__query_token,
-            'params': kwargs,
-            'fields': fields
+            'params': kwargs
         }
-
-        res = requests.post(self.__query_url, json=req_params, timeout=self.__timeout, headers={'Connection': 'close'})
+        res = requests.post(self.__query_url, json=req_params, timeout=self.__timeout,
+                            headers={'Connection': 'close', 'Origin': 'https://sdk.doupand.com'})
         result = json.loads(res.text)
         if result['code'] != 0:
             raise Exception(result['msg'])
         data = result['data']
         columns = data['columns']
         values = data['values']
 
@@ -97,8 +100,8 @@
         直接将属性名称作为api_name传入query方法
         :param name:
         :return:
         """
         return partial(self.query, name)
 
 
-datareader = DataReader()
+data_reader = DataReader
```

### Comparing `doupand-1.0.3/doupand.egg-info/PKG-INFO` & `doupand-1.0.9/doupand.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doupand
-Version: 1.0.3
+Version: 1.0.9
 Summary: A simple and easy-to-use financial data interface library built for normal investors!
 Home-page: https://doupand.com
 Author: DouBro
 Author-email: doupand@163.com
 License: BSD
 Keywords: Financial Data Interface
 Platform: all
@@ -62,9 +62,7 @@
     4     000005.SZ  000005  ...         SZSE          主板
     ...         ...     ...  ...          ...         ...
     5329  873169.BJ  873169  ...          BSE         北交所
     5330  873223.BJ  873223  ...          BSE         北交所
     5331  873305.BJ  873305  ...          BSE         北交所
     5332  873339.BJ  873339  ...          BSE         北交所
     5333  873527.BJ  873527  ...          BSE         北交所
-
-
```

### Comparing `doupand-1.0.3/setup.py` & `doupand-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     5331  873305.BJ  873305  ...          BSE         北交所
     5332  873339.BJ  873339  ...          BSE         北交所
     5333  873527.BJ  873527  ...          BSE         北交所
 """
 
 setup(
     name='doupand',
-    version="1.0.3",
+    version="1.0.9",
     description='A simple and easy-to-use financial data interface library built for normal investors!',
     long_description=long_desc,
     author='DouBro',
     author_email='doupand@163.com',
     packages=find_packages(),
     platforms=["all"],
     license='BSD',
```

