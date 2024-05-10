# Comparing `tmp/PFlowC-2.0.0.tar.gz` & `tmp/PFlowC-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PFlowC-2.0.0.tar", last modified: Thu May  9 11:26:58 2024, max compression
+gzip compressed data, was "PFlowC-2.0.1.tar", last modified: Thu May  9 11:42:52 2024, max compression
```

## Comparing `PFlowC-2.0.0.tar` & `PFlowC-2.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:26:58.153543 PFlowC-2.0.0/
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:26:58.113946 PFlowC-2.0.0/PFlowC/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 10:53:34.000000 PFlowC-2.0.0/PFlowC/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3207 2024-05-09 03:46:04.000000 PFlowC-2.0.0/PFlowC/geo_proxy.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     7872 2024-04-29 09:28:01.000000 PFlowC-2.0.0/PFlowC/main.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      722 2024-04-28 09:32:05.000000 PFlowC-2.0.0/PFlowC/proxy.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:26:58.115196 PFlowC-2.0.0/PFlowC/proxy_helper/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      859 2024-04-29 09:50:09.000000 PFlowC-2.0.0/PFlowC/proxy_helper/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     7391 2024-04-29 09:49:45.000000 PFlowC-2.0.0/PFlowC/proxy_helper/macosx.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:26:58.150308 PFlowC-2.0.0/PFlowC/utils/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)  6381855 2024-04-29 05:46:08.000000 PFlowC-2.0.0/PFlowC/utils/Country.mmdb
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-2.0.0/PFlowC/utils/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-2.0.0/PFlowC/utils/logger.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     2000 2024-04-30 09:01:33.000000 PFlowC-2.0.0/PFlowC/utils/net.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:26:58.114822 PFlowC-2.0.0/PFlowC.egg-info/
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     2627 2024-05-09 11:26:57.000000 PFlowC-2.0.0/PFlowC.egg-info/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      588 2024-05-09 11:26:57.000000 PFlowC-2.0.0/PFlowC.egg-info/SOURCES.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-05-09 11:26:57.000000 PFlowC-2.0.0/PFlowC.egg-info/dependency_links.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-05-09 11:26:57.000000 PFlowC-2.0.0/PFlowC.egg-info/entry_points.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       15 2024-05-09 11:26:57.000000 PFlowC-2.0.0/PFlowC.egg-info/requires.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-05-09 11:26:57.000000 PFlowC-2.0.0/PFlowC.egg-info/top_level.txt
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     2627 2024-05-09 11:26:58.153218 PFlowC-2.0.0/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1667 2024-04-28 10:54:57.000000 PFlowC-2.0.0/README.rst
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-05-09 11:26:58.153607 PFlowC-2.0.0/setup.cfg
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1702 2024-04-30 08:23:30.000000 PFlowC-2.0.0/setup.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:26:58.152693 PFlowC-2.0.0/tests/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3532 2024-04-29 07:46:42.000000 PFlowC-2.0.0/tests/test-agent-service.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      416 2024-04-29 02:59:48.000000 PFlowC-2.0.0/tests/test-api.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      765 2024-04-28 10:17:38.000000 PFlowC-2.0.0/tests/test-banner.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      824 2024-04-30 04:51:51.000000 PFlowC-2.0.0/tests/test-dns-socket.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      858 2024-04-30 08:11:38.000000 PFlowC-2.0.0/tests/test-dnspython.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      566 2024-04-29 10:14:26.000000 PFlowC-2.0.0/tests/test-json-dump.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1313 2024-04-30 06:00:45.000000 PFlowC-2.0.0/tests/test-salary.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:42:52.412059 PFlowC-2.0.1/
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:42:52.391170 PFlowC-2.0.1/PFlowC/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-05-09 11:40:07.000000 PFlowC-2.0.1/PFlowC/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3212 2024-05-09 11:42:27.000000 PFlowC-2.0.1/PFlowC/geo_proxy.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     7872 2024-04-29 09:28:01.000000 PFlowC-2.0.1/PFlowC/main.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      722 2024-04-28 09:32:05.000000 PFlowC-2.0.1/PFlowC/proxy.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:42:52.392401 PFlowC-2.0.1/PFlowC/proxy_helper/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      859 2024-04-29 09:50:09.000000 PFlowC-2.0.1/PFlowC/proxy_helper/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     7391 2024-04-29 09:49:45.000000 PFlowC-2.0.1/PFlowC/proxy_helper/macosx.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:42:52.408681 PFlowC-2.0.1/PFlowC/utils/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)  6381855 2024-04-29 05:46:08.000000 PFlowC-2.0.1/PFlowC/utils/Country.mmdb
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-2.0.1/PFlowC/utils/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-2.0.1/PFlowC/utils/logger.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     2000 2024-04-30 09:01:33.000000 PFlowC-2.0.1/PFlowC/utils/net.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:42:52.392046 PFlowC-2.0.1/PFlowC.egg-info/
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     2791 2024-05-09 11:42:51.000000 PFlowC-2.0.1/PFlowC.egg-info/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      588 2024-05-09 11:42:51.000000 PFlowC-2.0.1/PFlowC.egg-info/SOURCES.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-05-09 11:42:51.000000 PFlowC-2.0.1/PFlowC.egg-info/dependency_links.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-05-09 11:42:51.000000 PFlowC-2.0.1/PFlowC.egg-info/entry_points.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       15 2024-05-09 11:42:51.000000 PFlowC-2.0.1/PFlowC.egg-info/requires.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-05-09 11:42:51.000000 PFlowC-2.0.1/PFlowC.egg-info/top_level.txt
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     2791 2024-05-09 11:42:52.411839 PFlowC-2.0.1/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1831 2024-05-09 11:41:01.000000 PFlowC-2.0.1/README.rst
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-05-09 11:42:52.412096 PFlowC-2.0.1/setup.cfg
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1702 2024-05-09 11:41:28.000000 PFlowC-2.0.1/setup.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-09 11:42:52.411329 PFlowC-2.0.1/tests/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3532 2024-04-29 07:46:42.000000 PFlowC-2.0.1/tests/test-agent-service.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      416 2024-04-29 02:59:48.000000 PFlowC-2.0.1/tests/test-api.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      765 2024-04-28 10:17:38.000000 PFlowC-2.0.1/tests/test-banner.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      824 2024-04-30 04:51:51.000000 PFlowC-2.0.1/tests/test-dns-socket.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      858 2024-04-30 08:11:38.000000 PFlowC-2.0.1/tests/test-dnspython.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      566 2024-04-29 10:14:26.000000 PFlowC-2.0.1/tests/test-json-dump.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1313 2024-04-30 06:00:45.000000 PFlowC-2.0.1/tests/test-salary.py
```

### Comparing `PFlowC-2.0.0/PFlowC/geo_proxy.py` & `PFlowC-2.0.1/PFlowC/geo_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     'doh.pub',
     'dns.alidns.com',
     "218.31.113.0/24"
 ]
 AGENT_DOMAINS = {
     "CN": [
         "github.com"
-        "api.github.com"]
+        "api.github.com"
+    ]
 }
 # 初始化GeoIP数据库
 geoip_db = geoip2.database.Reader(GEOIP_DB_PATH)
 home_dir = os.path.expanduser("~/.PFlowC")
 bypass_domains_fp = os.path.join(home_dir, "bypass_domains.json")
 bypass_domains = set()
 if not os.path.isfile(bypass_domains_fp):
```

### Comparing `PFlowC-2.0.0/PFlowC/main.py` & `PFlowC-2.0.1/PFlowC/main.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.0.0/PFlowC/proxy.py` & `PFlowC-2.0.1/PFlowC/proxy.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.0.0/PFlowC/proxy_helper/__init__.py` & `PFlowC-2.0.1/PFlowC/proxy_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.0.0/PFlowC/proxy_helper/macosx.py` & `PFlowC-2.0.1/PFlowC/proxy_helper/macosx.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.0.0/PFlowC/utils/Country.mmdb` & `PFlowC-2.0.1/PFlowC/utils/Country.mmdb`

 * *Files identical despite different names*

### Comparing `PFlowC-2.0.0/PFlowC/utils/logger.py` & `PFlowC-2.0.1/PFlowC/utils/logger.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.0.0/PFlowC/utils/net.py` & `PFlowC-2.0.1/PFlowC/utils/net.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.0.0/PFlowC.egg-info/PKG-INFO` & `PFlowC-2.0.1/PFlowC.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 2.0.0
+Version: 2.0.1
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,30 +38,35 @@
     ██╔══██╗██╔════╝██║     ██╔═══██╗██║    ██║██╔════╝
     ██████╔╝█████╗  ██║     ██║   ██║██║ █╗ ██║██║
     ██╔═══╝ ██╔══╝  ██║     ██║   ██║██║███╗██║██║
     ██║     ██║     ███████╗╚██████╔╝╚███╔███╔╝╚██████╗
     ╚═╝     ╚═╝     ╚══════╝ ╚═════╝  ╚══╝╚══╝  ╚═════╝
 
     Command line interface for Proxy Flow Controller with basic auto configurations.
-    Version: 1.4.0                    By: BlackHaoke<Haoke98@outlook.com>
-    Usage: main.py [OPTIONS] COMMAND [ARGS]...
+    Version: 2.0.1                    By: BlackHaoke<Haoke98@outlook.com>
+    Usage: pflow-cli [OPTIONS] COMMAND [ARGS]...
 
     Options:
       --help  Show this message and exit.
 
     Commands:
       off      Set off and clear all proxy config.
       on       Run proxy flow controller.
+      server   Server as the Agent service for the local device in same LAN...
       version  Version
 
-
 * Install:
 
     Run ``pip install PFlowC -U`` on the shell.
 
+* start a local flow control service:
+
+    Run ``pflow-cli server`` on the shell.
+
+
 * set on the proxy setting:
 
     Run ``pflow-cli on`` on the shell.
 
 * set off the proxy setting:
 
     Run ``pflow-cli off`` on the shell.
```

### Comparing `PFlowC-2.0.0/PFlowC.egg-info/SOURCES.txt` & `PFlowC-2.0.1/PFlowC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PFlowC-2.0.0/PKG-INFO` & `PFlowC-2.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 2.0.0
+Version: 2.0.1
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,30 +38,35 @@
     ██╔══██╗██╔════╝██║     ██╔═══██╗██║    ██║██╔════╝
     ██████╔╝█████╗  ██║     ██║   ██║██║ █╗ ██║██║
     ██╔═══╝ ██╔══╝  ██║     ██║   ██║██║███╗██║██║
     ██║     ██║     ███████╗╚██████╔╝╚███╔███╔╝╚██████╗
     ╚═╝     ╚═╝     ╚══════╝ ╚═════╝  ╚══╝╚══╝  ╚═════╝
 
     Command line interface for Proxy Flow Controller with basic auto configurations.
-    Version: 1.4.0                    By: BlackHaoke<Haoke98@outlook.com>
-    Usage: main.py [OPTIONS] COMMAND [ARGS]...
+    Version: 2.0.1                    By: BlackHaoke<Haoke98@outlook.com>
+    Usage: pflow-cli [OPTIONS] COMMAND [ARGS]...
 
     Options:
       --help  Show this message and exit.
 
     Commands:
       off      Set off and clear all proxy config.
       on       Run proxy flow controller.
+      server   Server as the Agent service for the local device in same LAN...
       version  Version
 
-
 * Install:
 
     Run ``pip install PFlowC -U`` on the shell.
 
+* start a local flow control service:
+
+    Run ``pflow-cli server`` on the shell.
+
+
 * set on the proxy setting:
 
     Run ``pflow-cli on`` on the shell.
 
 * set off the proxy setting:
 
     Run ``pflow-cli off`` on the shell.
```

### Comparing `PFlowC-2.0.0/setup.py` & `PFlowC-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 except ImportError:
     from distutils.core import setup
 
 long_description = open('README.rst').read()
 
 setup(
     name='PFlowC',
-    version='2.0.0',
+    version='2.0.1',
     url='https://github.com/Haoke98/FlowPilot',
     author='Haoke98',
     author_email='BlackHaoke<Haoke98@outlook.com>',
     license='MIT',
     description='https://github.com/Haoke98/FlowPilot/README.md',
     packages=["PFlowC", "PFlowC.utils", "PFlowC.proxy_helper"],
     install_requires=['colorlog', 'click'],
```

### Comparing `PFlowC-2.0.0/tests/test-agent-service.py` & `PFlowC-2.0.1/tests/test-agent-service.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.0.0/tests/test-banner.py` & `PFlowC-2.0.1/tests/test-banner.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.0.0/tests/test-dns-socket.py` & `PFlowC-2.0.1/tests/test-dns-socket.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.0.0/tests/test-dnspython.py` & `PFlowC-2.0.1/tests/test-dnspython.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.0.0/tests/test-json-dump.py` & `PFlowC-2.0.1/tests/test-json-dump.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.0.0/tests/test-salary.py` & `PFlowC-2.0.1/tests/test-salary.py`

 * *Files identical despite different names*

