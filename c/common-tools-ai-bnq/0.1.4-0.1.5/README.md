# Comparing `tmp/common-tools-ai-bnq-0.1.4.tar.gz` & `tmp/common-tools-ai-bnq-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-tools-ai-bnq-0.1.4.tar", last modified: Mon May  6 09:19:18 2024, max compression
+gzip compressed data, was "common-tools-ai-bnq-0.1.5.tar", last modified: Fri May 10 08:16:10 2024, max compression
```

## Comparing `common-tools-ai-bnq-0.1.4.tar` & `common-tools-ai-bnq-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 09:19:18.672875 common-tools-ai-bnq-0.1.4/
--rw-rw-rw-   0        0        0     2598 2024-05-06 09:19:18.671874 common-tools-ai-bnq-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2236 2024-04-24 02:51:54.000000 common-tools-ai-bnq-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 09:19:18.653149 common-tools-ai-bnq-0.1.4/bnq_py_core/
--rw-rw-rw-   0        0        0      356 2024-04-24 02:52:35.000000 common-tools-ai-bnq-0.1.4/bnq_py_core/__init__.py
--rw-rw-rw-   0        0        0     1088 2024-05-06 07:47:07.000000 common-tools-ai-bnq-0.1.4/bnq_py_core/cos_connect.py
--rw-rw-rw-   0        0        0     4566 2024-05-06 09:18:58.000000 common-tools-ai-bnq-0.1.4/bnq_py_core/logger_record.py
--rw-rw-rw-   0        0        0     3218 2024-05-06 09:03:26.000000 common-tools-ai-bnq-0.1.4/bnq_py_core/nacos_connect.py
--rw-rw-rw-   0        0        0     2074 2024-04-19 07:39:44.000000 common-tools-ai-bnq-0.1.4/bnq_py_core/read_conf_from_ini.py
--rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.1.4/bnq_py_core/singleton.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:19:18.670873 common-tools-ai-bnq-0.1.4/common_tools_ai_bnq.egg-info/
--rw-rw-rw-   0        0        0     2598 2024-05-06 09:19:18.000000 common-tools-ai-bnq-0.1.4/common_tools_ai_bnq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2024-05-06 09:19:18.000000 common-tools-ai-bnq-0.1.4/common_tools_ai_bnq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 09:19:18.000000 common-tools-ai-bnq-0.1.4/common_tools_ai_bnq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-05-06 09:19:18.000000 common-tools-ai-bnq-0.1.4/common_tools_ai_bnq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-06 09:19:18.000000 common-tools-ai-bnq-0.1.4/common_tools_ai_bnq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 09:19:18.672875 common-tools-ai-bnq-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      828 2024-05-06 09:19:13.000000 common-tools-ai-bnq-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:16:10.110012 common-tools-ai-bnq-0.1.5/
+-rw-rw-rw-   0        0        0     2511 2024-05-10 08:16:10.110012 common-tools-ai-bnq-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2304 2024-05-10 08:15:54.000000 common-tools-ai-bnq-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 08:16:10.089810 common-tools-ai-bnq-0.1.5/bnq_py_core/
+-rw-rw-rw-   0        0        0      356 2024-04-24 02:52:35.000000 common-tools-ai-bnq-0.1.5/bnq_py_core/__init__.py
+-rw-rw-rw-   0        0        0     1088 2024-05-06 07:47:07.000000 common-tools-ai-bnq-0.1.5/bnq_py_core/cos_connect.py
+-rw-rw-rw-   0        0        0     4616 2024-05-10 08:10:48.000000 common-tools-ai-bnq-0.1.5/bnq_py_core/logger_record.py
+-rw-rw-rw-   0        0        0     3218 2024-05-06 09:03:26.000000 common-tools-ai-bnq-0.1.5/bnq_py_core/nacos_connect.py
+-rw-rw-rw-   0        0        0     1995 2024-05-10 08:10:10.000000 common-tools-ai-bnq-0.1.5/bnq_py_core/read_conf_from_ini.py
+-rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.1.5/bnq_py_core/singleton.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:16:10.109019 common-tools-ai-bnq-0.1.5/common_tools_ai_bnq.egg-info/
+-rw-rw-rw-   0        0        0     2511 2024-05-10 08:16:09.000000 common-tools-ai-bnq-0.1.5/common_tools_ai_bnq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2024-05-10 08:16:10.000000 common-tools-ai-bnq-0.1.5/common_tools_ai_bnq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 08:16:09.000000 common-tools-ai-bnq-0.1.5/common_tools_ai_bnq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-05-10 08:16:09.000000 common-tools-ai-bnq-0.1.5/common_tools_ai_bnq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-10 08:16:09.000000 common-tools-ai-bnq-0.1.5/common_tools_ai_bnq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 08:16:10.111013 common-tools-ai-bnq-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      828 2024-05-10 08:16:06.000000 common-tools-ai-bnq-0.1.5/setup.py
```

### Comparing `common-tools-ai-bnq-0.1.4/PKG-INFO` & `common-tools-ai-bnq-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: common-tools-ai-bnq
-Version: 0.1.4
+Version: 0.1.5
 Summary: Common tools of AI module for BNQ
 Author: BNQ
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: structlog==23.1.0
-Requires-Dist: concurrent-log-handler==0.9.22
-Requires-Dist: nacos-sdk-python==0.1.12
-Requires-Dist: PyYAML==6.0.1
-Requires-Dist: cos-python-sdk-v5==1.9.28
+
+    python setup.py sdist bdist_wheel
+    twine upload dist/*
+
 
 1.NacConnect类，用于连接nacos服务，获取配置文件信息
 
     NacConnect类中参数信息如下：
         server_addresses: 地址
         namespace: 命名空间
         username: 用户名
@@ -68,7 +69,8 @@
         test_data = {
                         'secret_id': 'AKIDxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',
                         'secret_key': 'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',
                         'region': 'ap-guangzhou'
                     }
         cos_test = CosConnect(**test_data)
         print(cos_test())
+
```

### Comparing `common-tools-ai-bnq-0.1.4/README.md` & `common-tools-ai-bnq-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+    python setup.py sdist bdist_wheel
+    twine upload dist/*
+
+
 1.NacConnect类，用于连接nacos服务，获取配置文件信息
 
     NacConnect类中参数信息如下：
         server_addresses: 地址
         namespace: 命名空间
         username: 用户名
         password: 密码
```

### Comparing `common-tools-ai-bnq-0.1.4/bnq_py_core/cos_connect.py` & `common-tools-ai-bnq-0.1.5/bnq_py_core/cos_connect.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.4/bnq_py_core/logger_record.py` & `common-tools-ai-bnq-0.1.5/bnq_py_core/logger_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,16 @@
         """初始化log模块
 
         Returns:
 
         """
         if self.log_record_path is None:
             # 获取根目录路径，并创建日志文件夹
-            self.log_record_path = os.path.join(os.getcwd(), "logs")
+            # self.log_record_path = os.path.join(os.getcwd(), "logs")
+            self.log_record_path = "/bnq/logs"
 
         pathlib.Path(self.log_record_path).mkdir(parents=True, exist_ok=True)
         log_filename = os.path.join(self.log_record_path, self.__filename)
         logging.config.dictConfig({
             "version": 1,
             "disable_existing_loggers": False,
             "formatters": {
```

### Comparing `common-tools-ai-bnq-0.1.4/bnq_py_core/nacos_connect.py` & `common-tools-ai-bnq-0.1.5/bnq_py_core/nacos_connect.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.4/bnq_py_core/read_conf_from_ini.py` & `common-tools-ai-bnq-0.1.5/bnq_py_core/read_conf_from_ini.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,16 +23,15 @@
         """
         if not cls.__instance:
             cls.__instance = super(GetConfInfo, cls).__new__(cls, *args, **kwargs)
         return cls.__instance
 
     def __init__(self):
         self.conf = configparser.RawConfigParser()
-        path_file = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-        self.conf_path = os.path.join(path_file, "config", "conf.ini")
+        self.conf_path = os.path.join(os.getcwd(), "config", "conf.ini")
         self.conf.read(self.conf_path)
         log_env_path = os.path.join(path_file, 'logenv')
         self.field = self.get_field(log_env_path)
 
     @staticmethod
     def get_field(log_env_path):
         """根据log env记录的值，获取不同环境的配置参数
```

### Comparing `common-tools-ai-bnq-0.1.4/bnq_py_core/singleton.py` & `common-tools-ai-bnq-0.1.5/bnq_py_core/singleton.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.4/common_tools_ai_bnq.egg-info/PKG-INFO` & `common-tools-ai-bnq-0.1.5/common_tools_ai_bnq.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: common-tools-ai-bnq
-Version: 0.1.4
+Version: 0.1.5
 Summary: Common tools of AI module for BNQ
 Author: BNQ
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: structlog==23.1.0
-Requires-Dist: concurrent-log-handler==0.9.22
-Requires-Dist: nacos-sdk-python==0.1.12
-Requires-Dist: PyYAML==6.0.1
-Requires-Dist: cos-python-sdk-v5==1.9.28
+
+    python setup.py sdist bdist_wheel
+    twine upload dist/*
+
 
 1.NacConnect类，用于连接nacos服务，获取配置文件信息
 
     NacConnect类中参数信息如下：
         server_addresses: 地址
         namespace: 命名空间
         username: 用户名
@@ -68,7 +69,8 @@
         test_data = {
                         'secret_id': 'AKIDxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',
                         'secret_key': 'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',
                         'region': 'ap-guangzhou'
                     }
         cos_test = CosConnect(**test_data)
         print(cos_test())
+
```

### Comparing `common-tools-ai-bnq-0.1.4/setup.py` & `common-tools-ai-bnq-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='common-tools-ai-bnq',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     install_requires=[
         # 依赖项列表
         'structlog==23.1.0',
         'concurrent-log-handler==0.9.22',
         'nacos-sdk-python==0.1.12',
         'PyYAML==6.0.1',
```

