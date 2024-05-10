# Comparing `tmp/tsugu-api-python-0.2.0.tar.gz` & `tmp/tsugu-api-python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-api-python-0.2.0.tar", last modified: Mon May  6 07:59:17 2024, max compression
+gzip compressed data, was "tsugu-api-python-0.2.1.tar", last modified: Fri May 10 07:15:30 2024, max compression
```

## Comparing `tsugu-api-python-0.2.0.tar` & `tsugu-api-python-0.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/tsugu_api/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/tsugu_api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/v1/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/v1/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/v1/_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/tsugu_api/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/v2/_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/tsugu_api_async/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/tsugu_api_async/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/v1/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/v1/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/v1/_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/tsugu_api_async/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/v2/_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/tsugu_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-06 07:59:17.000000 tsugu-api-python-0.2.0/tsugu_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-06 07:59:17.000000 tsugu-api-python-0.2.0/tsugu_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:59:17.000000 tsugu-api-python-0.2.0/tsugu_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 07:59:17.000000 tsugu-api-python-0.2.0/tsugu_api_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:15:30.557793 tsugu-api-python-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-10 07:15:30.557793 tsugu-api-python-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 07:15:30.557793 tsugu-api-python-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:15:30.553793 tsugu-api-python-0.2.1/tsugu_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:15:30.553793 tsugu-api-python-0.2.1/tsugu_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/v1/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/v1/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/v1/_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:15:30.553793 tsugu-api-python-0.2.1/tsugu_api/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api/v2/_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:15:30.557793 tsugu-api-python-0.2.1/tsugu_api_async/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:15:30.557793 tsugu-api-python-0.2.1/tsugu_api_async/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/v1/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/v1/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/v1/_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:15:30.557793 tsugu-api-python-0.2.1/tsugu_api_async/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-10 07:15:21.000000 tsugu-api-python-0.2.1/tsugu_api_async/v2/_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:15:30.557793 tsugu-api-python-0.2.1/tsugu_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-10 07:15:30.000000 tsugu-api-python-0.2.1/tsugu_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-10 07:15:30.000000 tsugu-api-python-0.2.1/tsugu_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:15:30.000000 tsugu-api-python-0.2.1/tsugu_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 07:15:30.000000 tsugu-api-python-0.2.1/tsugu_api_python.egg-info/top_level.txt
```

### Comparing `tsugu-api-python-0.2.0/LICENSE` & `tsugu-api-python-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/PKG-INFO` & `tsugu-api-python-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 0.2.0 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 0.2.1 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-0.2.0/README.md` & `tsugu-api-python-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/setup.py` & `tsugu-api-python-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu-api-python',
-    version='0.2.0',
+    version='0.2.1',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Tsugu BanGDream Bot 的功能 API 统合包',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/tsugu-api-python',
     include_package_data=False,
```

### Comparing `tsugu-api-python-0.2.0/tsugu_api/_network.py` & `tsugu-api-python-0.2.1/tsugu_api/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/tsugu_api/_typing.py` & `tsugu-api-python-0.2.1/tsugu_api/_typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     default_server: list[_Server]
     car: bool
     server_list: list[_ServerData]
 
 class _UserDataResult(TypedDict):
     '''`get_user_data` 响应结果'''
     status: _Status
-    data: Union[str, list[_UserData]]
+    data: Union[str, _UserData]
 
 class _VerifyCode(TypedDict):
     '''验证码'''
     verifyCode: int
 
 class _BindResponse(TypedDict):
     '''绑定响应'''
```

### Comparing `tsugu-api-python-0.2.0/tsugu_api/settings.py` & `tsugu-api-python-0.2.1/tsugu_api/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/tsugu_api/utils.py` & `tsugu-api-python-0.2.1/tsugu_api/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/tsugu_api/v1/__init__.py` & `tsugu-api-python-0.2.1/tsugu_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/tsugu_api/v1/_bandoristation.py` & `tsugu-api-python-0.2.1/tsugu_api/v1/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/tsugu_api/v1/_tsugu.py` & `tsugu-api-python-0.2.1/tsugu_api/v1/_tsugu.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,33 +33,36 @@
     # 发送请求
     return Api(
         url,
         proxy=settings.backend_proxy,
         data=data
     ).post().json()
 
-def gacha_simulate(server_mode: _Server, gacha_id: Optional[int] = None) -> _Response:
+def gacha_simulate(server_mode: _Server, times: Optional[int] = None, gacha_id: Optional[int] = None) -> _Response:
     '''模拟抽卡
 
     参数:
         server_mode (_Server): 服务器模式
+        times (int): 抽卡次数
         gacha_id (int): 卡池 ID
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
     url = settings.backend_url + '/gachaSimulate'
     
     # 构建数据
     data = {
         'server_mode': server_mode,
         'compress': settings.compress
     }
+    if times:
+        data['times'] = times
     if gacha_id:
         data['gachaId'] = gacha_id
     
     # 发送请求
     return Api(
         url,
         proxy=settings.backend_proxy,
```

### Comparing `tsugu-api-python-0.2.0/tsugu_api/v1/_user.py` & `tsugu-api-python-0.2.1/tsugu_api/v1/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/tsugu_api/v2/__init__.py` & `tsugu-api-python-0.2.1/tsugu_api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/tsugu_api/v2/_api.py` & `tsugu-api-python-0.2.1/tsugu_api/v2/_api.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/tsugu_api_async/_network.py` & `tsugu-api-python-0.2.1/tsugu_api_async/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/tsugu_api_async/_typing.py` & `tsugu-api-python-0.2.1/tsugu_api_async/_typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     default_server: list[_Server]
     car: bool
     server_list: list[_ServerData]
 
 class _UserDataResult(TypedDict):
     '''`get_user_data` 响应结果'''
     status: _Status
-    data: Union[str, list[_UserData]]
+    data: Union[str, _UserData]
 
 class _VerifyCode(TypedDict):
     '''验证码'''
     verifyCode: int
 
 class _BindResponse(TypedDict):
     '''绑定响应'''
```

### Comparing `tsugu-api-python-0.2.0/tsugu_api_async/settings.py` & `tsugu-api-python-0.2.1/tsugu_api_async/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/tsugu_api_async/utils.py` & `tsugu-api-python-0.2.1/tsugu_api_async/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/tsugu_api_async/v1/__init__.py` & `tsugu-api-python-0.2.1/tsugu_api_async/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/tsugu_api_async/v1/_bandoristation.py` & `tsugu-api-python-0.2.1/tsugu_api_async/v1/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/tsugu_api_async/v1/_tsugu.py` & `tsugu-api-python-0.2.1/tsugu_api_async/v1/_tsugu.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,33 +38,36 @@
         url,
         proxy=settings.backend_proxy,
         data=data
     ).post()
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def gacha_simulate(server_mode: _Server, gacha_id: Optional[int] = None) -> _Response:
+async def gacha_simulate(server_mode: _Server, times: Optional[int] = None, gacha_id: Optional[int] = None) -> _Response:
     '''模拟抽卡
 
     参数:
         server_mode (_Server): 服务器模式
+        times (int): 抽卡次数
         gacha_id (int): 卡池 ID
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
     url = settings.backend_url + '/gachaSimulate'
     
     # 构建数据
     data = {
         'server_mode': server_mode,
         'compress': settings.compress
     }
+    if times:
+        data['times'] = times
     if gacha_id:
         data['gachaId'] = gacha_id
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.backend_proxy,
```

### Comparing `tsugu-api-python-0.2.0/tsugu_api_async/v1/_user.py` & `tsugu-api-python-0.2.1/tsugu_api_async/v1/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/tsugu_api_async/v2/__init__.py` & `tsugu-api-python-0.2.1/tsugu_api_async/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/tsugu_api_async/v2/_api.py` & `tsugu-api-python-0.2.1/tsugu_api_async/v2/_api.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.0/tsugu_api_python.egg-info/PKG-INFO` & `tsugu-api-python-0.2.1/tsugu_api_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 0.2.0 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 0.2.1 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-0.2.0/tsugu_api_python.egg-info/SOURCES.txt` & `tsugu-api-python-0.2.1/tsugu_api_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

