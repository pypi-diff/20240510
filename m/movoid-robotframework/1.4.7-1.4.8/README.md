# Comparing `tmp/movoid_robotframework-1.4.7.tar.gz` & `tmp/movoid_robotframework-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_robotframework-1.4.7.tar", last modified: Thu May  9 13:04:52 2024, max compression
+gzip compressed data, was "movoid_robotframework-1.4.8.tar", last modified: Fri May 10 20:23:08 2024, max compression
```

## Comparing `movoid_robotframework-1.4.7.tar` & `movoid_robotframework-1.4.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 13:04:52.926026 movoid_robotframework-1.4.7/
--rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0      290 2024-05-09 13:04:52.923992 movoid_robotframework-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework-1.4.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 13:04:52.909659 movoid_robotframework-1.4.7/RobotFrameworkBasic/
--rw-rw-rw-   0        0        0      451 2024-02-20 17:41:03.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:04:52.914775 movoid_robotframework-1.4.7/RobotFrameworkBasic/action/
--rw-rw-rw-   0        0        0      253 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/action/__init__.py
--rw-rw-rw-   0        0        0     7070 2024-02-20 17:45:15.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/action/calculate.py
--rw-rw-rw-   0        0        0     9735 2024-05-09 13:02:53.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/action/config.py
--rw-rw-rw-   0        0        0     6810 2024-05-06 14:37:08.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/common.py
--rw-rw-rw-   0        0        0    14138 2024-04-20 15:07:13.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/decorator.py
--rw-rw-rw-   0        0        0      497 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/error.py
--rw-rw-rw-   0        0        0      286 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/main.py
--rw-rw-rw-   0        0        0      911 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/version.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:04:52.922971 movoid_robotframework-1.4.7/movoid_robotframework.egg-info/
--rw-rw-rw-   0        0        0      290 2024-05-09 13:04:52.000000 movoid_robotframework-1.4.7/movoid_robotframework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-05-09 13:04:52.000000 movoid_robotframework-1.4.7/movoid_robotframework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 13:04:52.000000 movoid_robotframework-1.4.7/movoid_robotframework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-09 13:04:52.000000 movoid_robotframework-1.4.7/movoid_robotframework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-05-09 13:04:52.000000 movoid_robotframework-1.4.7/movoid_robotframework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 13:04:52.926026 movoid_robotframework-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0      558 2024-05-09 13:04:15.000000 movoid_robotframework-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:23:08.847076 movoid_robotframework-1.4.8/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      290 2024-05-10 20:23:08.846077 movoid_robotframework-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework-1.4.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 20:23:08.833090 movoid_robotframework-1.4.8/RobotFrameworkBasic/
+-rw-rw-rw-   0        0        0      451 2024-02-20 17:41:03.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:23:08.837077 movoid_robotframework-1.4.8/RobotFrameworkBasic/action/
+-rw-rw-rw-   0        0        0      253 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/action/__init__.py
+-rw-rw-rw-   0        0        0     7070 2024-02-20 17:45:15.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/action/calculate.py
+-rw-rw-rw-   0        0        0     9917 2024-05-10 20:17:13.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/action/config.py
+-rw-rw-rw-   0        0        0     8155 2024-05-10 20:17:13.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/common.py
+-rw-rw-rw-   0        0        0    14138 2024-04-20 15:07:13.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/decorator.py
+-rw-rw-rw-   0        0        0      497 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/error.py
+-rw-rw-rw-   0        0        0      286 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/main.py
+-rw-rw-rw-   0        0        0      911 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.8/RobotFrameworkBasic/version.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:23:08.845050 movoid_robotframework-1.4.8/movoid_robotframework.egg-info/
+-rw-rw-rw-   0        0        0      290 2024-05-10 20:23:08.000000 movoid_robotframework-1.4.8/movoid_robotframework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-05-10 20:23:08.000000 movoid_robotframework-1.4.8/movoid_robotframework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 20:23:08.000000 movoid_robotframework-1.4.8/movoid_robotframework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-10 20:23:08.000000 movoid_robotframework-1.4.8/movoid_robotframework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-10 20:23:08.000000 movoid_robotframework-1.4.8/movoid_robotframework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 20:23:08.847076 movoid_robotframework-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      558 2024-05-10 20:22:31.000000 movoid_robotframework-1.4.8/setup.py
```

### Comparing `movoid_robotframework-1.4.7/RobotFrameworkBasic/action/calculate.py` & `movoid_robotframework-1.4.8/RobotFrameworkBasic/action/calculate.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.7/RobotFrameworkBasic/action/config.py` & `movoid_robotframework-1.4.8/RobotFrameworkBasic/action/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,30 +47,35 @@
 
 
 class Config:
     __suite_case_label = '__suit_case__'
     __suite_case_platform_label = f'__suit_case_{platform.system()}__'
 
     def __init__(self, json_file: str = None, print_func=None):
-        self._path = Path('config.json')
+        self._path = Path('robot_config.json')
         self._ori: Dict[str, Dict[str, Any]] = {}
         self._now: Dict[str, ConfigItem] = {}
         self._label_list: List[str] = []
-        self.init(json_file)
+        self.init(json_file, False)
         self.print = print if print_func is None else print_func
 
     def __contains__(self, item):
         return item in self._now
 
     def __getitem__(self, item):
         return self._now[item].value
 
-    def init(self, json_file: str = None):
+    def get(self, item, default=None):
+        return self._now[item].value if item in self._now else default
+
+    def init(self, json_file: str = None, new: bool = True):
         self._path = self._path if json_file is None else Path(json_file)
-        self.read()
+        if new or self._path.exists():
+            self.read()
+            self.use_suite_case_list('__init__')
 
     def write(self):
         temp_dict = {_k: _v for _k, _v in self._ori.items() if not _k.startswith('$')}
         with self._path.open(mode='w') as f:
             json.dump(temp_dict, f, default=lambda x: x.value, indent=2)
         temp_path = self._path.parent / f'${self._path.name}'
         temp_dict2 = {_k: _v for _k, _v in self._ori.items() if _k.startswith('$')}
@@ -189,55 +194,55 @@
             self.now_use_label(label, override=override, clear=False)
 
 
 class BasicConfig(BasicCommon):
 
     def __init__(self):
         super().__init__()
-        self._config_config = Config(print_func=self.print)
-        self.set_robot_variable('_config', self._config_config)
+        self.config = Config(print_func=self.print)
+        self.set_robot_variable('config', self.config)
 
     @robot_log_keyword
     def config_init(self, json_file: str = None):
         """
         初始化json文件，相当于重新选择json文件并读取生效
         :param json_file: json文件的路径，可以绝对可以相对，没有该文件的情况下保存会新建一个
         """
-        self._config_config.init(json_file)
+        self.config.init(json_file)
 
     @robot_log_keyword
     def config_use_label(self, *labels: str, override: bool = True, clear: bool = False):
         """
         选择相应的label生效
         :param labels: 待选择的label，必须是json文件里的
         :param override: 如果某个key已经存在，那么新数据是否覆盖就数据，默认覆盖
         :param clear: 是否将之前生效的所有数据全部删除
         """
         for label in labels:
-            self._config_config.now_use_label(label, override=override, clear=clear)
+            self.config.now_use_label(label, override=override, clear=clear)
 
     @robot_log_keyword
     def config_show_now_value(self):
         """
         显示当前使用的所有的键值
         """
-        self._config_config.show_now_value()
+        self.config.show_now_value()
 
     @robot_log_keyword
     def config_show_now_list(self):
         """
         显示当前使用的所有的label名
         """
-        self._config_config.show_now_list()
+        self.config.show_now_list()
 
     @robot_log_keyword
     def config_use_suite_case_list(self, custom_key: str = '', override: bool = True, clear: bool = False):
         """
         使用特定key下的label list作为label并生效
         :param custom_key: 如果想要自定义key的话，可以输入字符串，否则使用suite-case的字符串作为key
         :param override: 如果使用的某个key已经存在，那么是否使用全新的参数进行覆盖，默认进行覆盖
         :param clear: 是否把就有的所有参数全部清除，可以删除一些没有太有必要的参数
         """
-        suite_case_key = custom_key if custom_key else self.get_suite_case_str()
-        self._config_config.use_suite_case_list(suite_case_key, override=override, clear=clear)
-        self._config_config.show_now_list()
-        self._config_config.show_now_value()
+        suite_case_key = custom_key if custom_key else self.get_suite_case_str(suite_ori='main')
+        self.config.use_suite_case_list(suite_case_key, override=override, clear=clear)
+        self.config.show_now_list()
+        self.config.show_now_value()
```

### Comparing `movoid_robotframework-1.4.7/RobotFrameworkBasic/common.py` & `movoid_robotframework-1.4.8/RobotFrameworkBasic/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # File          : common
 # Author        : Sun YiFan-Movoid
 # Time          : 2024/2/13 12:04
 # Description   : 
 """
 import base64
 import json
+import pathlib
 import traceback
 from typing import Union
 
 from robot.libraries.BuiltIn import BuiltIn
 
 from .decorator import robot_log_keyword
 from .error import RfError
@@ -23,51 +24,95 @@
 
 class BasicCommon:
     def __init__(self):
         super().__init__()
         self.built = BuiltIn()
         self.warn_list = []
         self.output_dir = getattr(self, 'output_dir', None)
+        self._robot_variable = {}
 
     if VERSION:
         print_function = {
             'DEBUG': logger.debug,
             'INFO': logger.info,
             'WARN': logger.warn,
             'ERROR': logger.error,
         }
 
         def print(self, *args, html=False, level='INFO', sep=' ', end='\n'):
             print_text = str(sep).join([str(_) for _ in args]) + str(end)
             self.print_function.get(level.upper(), logger.info)(print_text, html)
+
+        @robot_log_keyword
+        def get_robot_variable(self, variable_name: str, default=None):
+            return self.built.get_variable_value("${" + variable_name + "}", default)
+
+        @robot_log_keyword
+        def set_robot_variable(self, variable_name: str, value):
+            self.built.set_global_variable("${" + variable_name + "}", value)
+
+        @robot_log_keyword
+        def get_suite_case_str(self, join_str: str = '-', suite: bool = True, case: bool = True, suite_ori: str = ''):
+            """
+            获取当前的suit、case的名称
+            :param join_str: suite和case的连接字符串，默认为-
+            :param suite: 是否显示suite名
+            :param case: 是否显示case名，如果不是case内，即使True也不显示
+            :param suite_ori: suite名的最高suite是不是使用原名，如果设置为空，那么使用原名
+            :return: 连接好的字符串
+            """
+            sc_list = []
+            if suite:
+                suite = self.get_robot_variable('SUITE NAME')
+                if suite_ori:
+                    exe_dir = self.get_robot_variable('EXECDIR')
+                    main_suite_len = len(pathlib.Path(exe_dir).name)
+                    if len(suite) >= main_suite_len:
+                        suite_body = suite[main_suite_len:]
+                    else:
+                        suite_body = ''
+                    suite_head = suite_ori
+                    suite = suite_head + suite_body
+                sc_list.append(suite)
+            if case:
+                temp = self.get_robot_variable('TEST NAME')
+                if temp is not None:
+                    sc_list.append(self.get_robot_variable('TEST NAME'))
+            return join_str.join(sc_list)
     else:
         def print(self, *args, html=False, level='INFO', sep=' ', end='\n'):
             print(*args, sep=sep, end=end)
 
+        def get_robot_variable(self, variable_name: str, default=None):
+            return self._robot_variable.get(variable_name, default)
+
+        def set_robot_variable(self, variable_name: str, value):
+            self._robot_variable[variable_name] = value
+
+        def get_suite_case_str(self, join_str: str = '-', suite: bool = True, case: bool = True, suite_ori: str = ''):
+            sc_list = []
+            if suite:
+                sc_list.append('suite')
+            if case:
+                sc_list.append('case')
+            return join_str.join(sc_list)
+
     def debug(self, *args, html=False, sep=' ', end='\n'):
         self.print(*args, html=html, level='DEBUG', sep=sep, end=end)
 
     def info(self, *args, html=False, sep=' ', end='\n'):
         self.print(*args, html=html, level='INFO', sep=sep, end=end)
 
     def warn(self, *args, html=False, sep=' ', end='\n'):
         self.print(*args, html=html, level='WARN', sep=sep, end=end)
 
     def error(self, *args, html=False, sep=' ', end='\n'):
         self.print(*args, html=html, level='ERROR', sep=sep, end=end)
 
     @robot_log_keyword
-    def get_robot_variable(self, variable_name: str, default=None):
-        return self.built.get_variable_value("${" + variable_name + "}", default)
-
-    @robot_log_keyword
-    def set_robot_variable(self, variable_name: str, value):
-        self.built.set_global_variable("${" + variable_name + "}", value)
-
-    @robot_log_keyword
     def analyse_json(self, value):
         """
         change json str to a python value or do not change it
         :param value: a json str or anything
         :return: a python value or value itself
         """
         self.print(f'try to change str to variable:({type(value).__name__}):{value}')
@@ -109,32 +154,14 @@
         """
         ori_dict[key] = value
 
     def always_true(self):
         return True
 
     @robot_log_keyword
-    def get_suite_case_str(self, join_str: str = '-', suite: bool = True, case: bool = True):
-        """
-        获取当前的suit、case的名称
-        :param join_str: suite和case的连接字符串，默认为-
-        :param suite: 是否显示suite名
-        :param case: 是否显示case名，如果不是case内，即使True也不显示
-        :return: 连接好的字符串
-        """
-        sc_list = []
-        if suite:
-            sc_list.append(self.get_robot_variable('SUITE NAME'))
-        if case:
-            temp = self.get_robot_variable('TEST NAME')
-            if temp is not None:
-                sc_list.append(self.get_robot_variable('TEST NAME'))
-        return join_str.join(sc_list)
-
-    @robot_log_keyword
     def log_show_image(self, image_path: str):
         with open(image_path, mode='rb') as f:
             img_str = base64.b64encode(f.read()).decode()
             self.print(f'<img src="data:image/png;base64,{img_str}">', html=True)
 
     @robot_log_keyword
     def robot_check_param(self, param_str: object, param_style: Union[str, type], default=None, error=False):
```

### Comparing `movoid_robotframework-1.4.7/RobotFrameworkBasic/decorator.py` & `movoid_robotframework-1.4.8/RobotFrameworkBasic/decorator.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.7/RobotFrameworkBasic/version.py` & `movoid_robotframework-1.4.8/RobotFrameworkBasic/version.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.7/movoid_robotframework.egg-info/SOURCES.txt` & `movoid_robotframework-1.4.8/movoid_robotframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.7/setup.py` & `movoid_robotframework-1.4.8/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='movoid_robotframework',
-    version='1.4.7',
+    version='1.4.8',
     packages=find_packages(),
     url='',
     license='',
     author='movoid',
     author_email='bobrobotsun@163.com',
     description='',
     long_description=long_description,
```

