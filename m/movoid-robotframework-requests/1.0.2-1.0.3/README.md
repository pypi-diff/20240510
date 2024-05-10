# Comparing `tmp/movoid_robotframework_requests-1.0.2.tar.gz` & `tmp/movoid_robotframework_requests-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_robotframework_requests-1.0.2.tar", last modified: Thu May  9 13:05:26 2024, max compression
+gzip compressed data, was "movoid_robotframework_requests-1.0.3.tar", last modified: Fri May 10 20:23:20 2024, max compression
```

## Comparing `movoid_robotframework_requests-1.0.2.tar` & `movoid_robotframework_requests-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 13:05:26.323564 movoid_robotframework_requests-1.0.2/
--rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework_requests-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      417 2024-05-09 13:05:26.322497 movoid_robotframework_requests-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework_requests-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 13:05:26.298182 movoid_robotframework_requests-1.0.2/RobotFrameworkRequests/
--rw-rw-rw-   0        0        0      391 2024-05-09 13:02:51.000000 movoid_robotframework_requests-1.0.2/RobotFrameworkRequests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:05:26.306443 movoid_robotframework_requests-1.0.2/RobotFrameworkRequests/lib/
--rw-rw-rw-   0        0        0      267 2024-02-21 12:27:00.000000 movoid_robotframework_requests-1.0.2/RobotFrameworkRequests/lib/__init__.py
--rw-rw-rw-   0        0        0     2757 2024-05-08 15:36:43.000000 movoid_robotframework_requests-1.0.2/RobotFrameworkRequests/lib/requests.py
--rw-rw-rw-   0        0        0      405 2024-05-08 15:36:43.000000 movoid_robotframework_requests-1.0.2/RobotFrameworkRequests/lib/type.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:05:26.311647 movoid_robotframework_requests-1.0.2/RobotFrameworkRequests/main/
--rw-rw-rw-   0        0        0      275 2024-02-21 12:15:19.000000 movoid_robotframework_requests-1.0.2/RobotFrameworkRequests/main/__init__.py
--rw-rw-rw-   0        0        0      260 2024-05-08 15:53:44.000000 movoid_robotframework_requests-1.0.2/RobotFrameworkRequests/main/action.py
--rw-rw-rw-   0        0        0     3153 2024-05-09 13:02:51.000000 movoid_robotframework_requests-1.0.2/RobotFrameworkRequests/main/common.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:05:26.320299 movoid_robotframework_requests-1.0.2/movoid_robotframework_requests.egg-info/
--rw-rw-rw-   0        0        0      417 2024-05-09 13:05:26.000000 movoid_robotframework_requests-1.0.2/movoid_robotframework_requests.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      563 2024-05-09 13:05:26.000000 movoid_robotframework_requests-1.0.2/movoid_robotframework_requests.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 13:05:26.000000 movoid_robotframework_requests-1.0.2/movoid_robotframework_requests.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2024-05-09 13:05:26.000000 movoid_robotframework_requests-1.0.2/movoid_robotframework_requests.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-09 13:05:26.000000 movoid_robotframework_requests-1.0.2/movoid_robotframework_requests.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 13:05:26.323564 movoid_robotframework_requests-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      726 2024-05-09 13:05:01.000000 movoid_robotframework_requests-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:23:20.528852 movoid_robotframework_requests-1.0.3/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework_requests-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      417 2024-05-10 20:23:20.527847 movoid_robotframework_requests-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework_requests-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 20:23:20.504609 movoid_robotframework_requests-1.0.3/RobotFrameworkRequests/
+-rw-rw-rw-   0        0        0      391 2024-05-09 13:02:51.000000 movoid_robotframework_requests-1.0.3/RobotFrameworkRequests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:23:20.513442 movoid_robotframework_requests-1.0.3/RobotFrameworkRequests/lib/
+-rw-rw-rw-   0        0        0      267 2024-02-21 12:27:00.000000 movoid_robotframework_requests-1.0.3/RobotFrameworkRequests/lib/__init__.py
+-rw-rw-rw-   0        0        0     2757 2024-05-08 15:36:43.000000 movoid_robotframework_requests-1.0.3/RobotFrameworkRequests/lib/requests.py
+-rw-rw-rw-   0        0        0      405 2024-05-08 15:36:43.000000 movoid_robotframework_requests-1.0.3/RobotFrameworkRequests/lib/type.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:23:20.516913 movoid_robotframework_requests-1.0.3/RobotFrameworkRequests/main/
+-rw-rw-rw-   0        0        0      275 2024-02-21 12:15:19.000000 movoid_robotframework_requests-1.0.3/RobotFrameworkRequests/main/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-05-08 15:53:44.000000 movoid_robotframework_requests-1.0.3/RobotFrameworkRequests/main/action.py
+-rw-rw-rw-   0        0        0     3066 2024-05-10 20:17:16.000000 movoid_robotframework_requests-1.0.3/RobotFrameworkRequests/main/common.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:23:20.526770 movoid_robotframework_requests-1.0.3/movoid_robotframework_requests.egg-info/
+-rw-rw-rw-   0        0        0      417 2024-05-10 20:23:20.000000 movoid_robotframework_requests-1.0.3/movoid_robotframework_requests.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      563 2024-05-10 20:23:20.000000 movoid_robotframework_requests-1.0.3/movoid_robotframework_requests.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 20:23:20.000000 movoid_robotframework_requests-1.0.3/movoid_robotframework_requests.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2024-05-10 20:23:20.000000 movoid_robotframework_requests-1.0.3/movoid_robotframework_requests.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-10 20:23:20.000000 movoid_robotframework_requests-1.0.3/movoid_robotframework_requests.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 20:23:20.528852 movoid_robotframework_requests-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      726 2024-05-10 20:23:08.000000 movoid_robotframework_requests-1.0.3/setup.py
```

### Comparing `movoid_robotframework_requests-1.0.2/RobotFrameworkRequests/lib/requests.py` & `movoid_robotframework_requests-1.0.3/RobotFrameworkRequests/lib/requests.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework_requests-1.0.2/RobotFrameworkRequests/main/common.py` & `movoid_robotframework_requests-1.0.3/RobotFrameworkRequests/main/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,18 +28,18 @@
         self._request_param = {}
 
     @robot_log_keyword
     def api_url_check(self, url: str):
         if url.startswith('http'):
             return url
         else:
-            protocol_text = f'{self._config_config["protocol"]}://' if 'protocol' in self._config_config else 'http://'
-            ip_text = self._config_config["ip"] if "ip" in self._config_config else "127.0.0.1"
-            port_text = f':{self._config_config["port"]}' if "port" in self._config_config else ""
-            path_text = f"/{self._config_config['url_path_header'].strip('/')}" if "url_path_header" in self._config_config else ""
+            protocol_text = f'{self.config["protocol"]}://' if 'protocol' in self.config else 'http://'
+            ip_text = self.config.get("ip", "127.0.0.1")
+            port_text = f':{self.config["port"]}' if "port" in self.config else ""
+            path_text = f"/{self.config['url_path_header'].strip('/')}" if "url_path_header" in self.config else ""
             return f'{protocol_text}{ip_text}{port_text}{path_text}/' + url.lstrip('/')
 
     @robot_log_keyword
     def requests_ori(self, method, url, status=200, **kwargs):
         kwargs.setdefault('headers', self.headers)
         real_url = self.api_url_check(url)
         self._request_param = {'method': method, 'url': real_url, **kwargs}
```

### Comparing `movoid_robotframework_requests-1.0.2/movoid_robotframework_requests.egg-info/SOURCES.txt` & `movoid_robotframework_requests-1.0.3/movoid_robotframework_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `movoid_robotframework_requests-1.0.2/setup.py` & `movoid_robotframework_requests-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='movoid_robotframework_requests',
-    version='1.0.2',
+    version='1.0.3',
     packages=find_packages(),
     url='',
     license='',
     author='movoid',
     author_email='bobrobotsun@163.com',
     description='',
     long_description=long_description,
```

