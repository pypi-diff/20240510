# Comparing `tmp/PFlowC-2.1.0.tar.gz` & `tmp/PFlowC-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PFlowC-2.1.0.tar", last modified: Fri May 10 02:39:32 2024, max compression
+gzip compressed data, was "PFlowC-2.1.1.tar", last modified: Fri May 10 02:56:49 2024, max compression
```

## Comparing `PFlowC-2.1.0.tar` & `PFlowC-2.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 02:39:32.152744 PFlowC-2.1.0/
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 02:39:32.127247 PFlowC-2.1.0/PFlowC/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-05-10 02:35:17.000000 PFlowC-2.1.0/PFlowC/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3213 2024-05-10 02:34:22.000000 PFlowC-2.1.0/PFlowC/geo_proxy.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     7872 2024-04-29 09:28:01.000000 PFlowC-2.1.0/PFlowC/main.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      722 2024-04-28 09:32:05.000000 PFlowC-2.1.0/PFlowC/proxy.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 02:39:32.128541 PFlowC-2.1.0/PFlowC/proxy_helper/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      859 2024-04-29 09:50:09.000000 PFlowC-2.1.0/PFlowC/proxy_helper/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     7391 2024-04-29 09:49:45.000000 PFlowC-2.1.0/PFlowC/proxy_helper/macosx.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 02:39:32.149348 PFlowC-2.1.0/PFlowC/utils/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)  6381855 2024-04-29 05:46:08.000000 PFlowC-2.1.0/PFlowC/utils/Country.mmdb
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-2.1.0/PFlowC/utils/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-2.1.0/PFlowC/utils/logger.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     2000 2024-04-30 09:01:33.000000 PFlowC-2.1.0/PFlowC/utils/net.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 02:39:32.128186 PFlowC-2.1.0/PFlowC.egg-info/
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     2791 2024-05-10 02:39:31.000000 PFlowC-2.1.0/PFlowC.egg-info/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      617 2024-05-10 02:39:31.000000 PFlowC-2.1.0/PFlowC.egg-info/SOURCES.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-05-10 02:39:31.000000 PFlowC-2.1.0/PFlowC.egg-info/dependency_links.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-05-10 02:39:31.000000 PFlowC-2.1.0/PFlowC.egg-info/entry_points.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       15 2024-05-10 02:39:31.000000 PFlowC-2.1.0/PFlowC.egg-info/requires.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-05-10 02:39:31.000000 PFlowC-2.1.0/PFlowC.egg-info/top_level.txt
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     2791 2024-05-10 02:39:32.152517 PFlowC-2.1.0/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1831 2024-05-10 02:37:56.000000 PFlowC-2.1.0/README.rst
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-05-10 02:39:32.152788 PFlowC-2.1.0/setup.cfg
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1720 2024-05-10 02:36:15.000000 PFlowC-2.1.0/setup.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 02:39:32.151963 PFlowC-2.1.0/tests/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3532 2024-04-29 07:46:42.000000 PFlowC-2.1.0/tests/test-agent-service.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      416 2024-04-29 02:59:48.000000 PFlowC-2.1.0/tests/test-api.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      765 2024-04-28 10:17:38.000000 PFlowC-2.1.0/tests/test-banner.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      824 2024-04-30 04:51:51.000000 PFlowC-2.1.0/tests/test-dns-socket.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      858 2024-04-30 08:11:38.000000 PFlowC-2.1.0/tests/test-dnspython.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      532 2024-05-10 02:34:13.000000 PFlowC-2.1.0/tests/test-filter-domains.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      566 2024-04-29 10:14:26.000000 PFlowC-2.1.0/tests/test-json-dump.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1313 2024-04-30 06:00:45.000000 PFlowC-2.1.0/tests/test-salary.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 02:56:49.261865 PFlowC-2.1.1/
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 02:56:49.234214 PFlowC-2.1.1/PFlowC/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-05-10 02:51:14.000000 PFlowC-2.1.1/PFlowC/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3213 2024-05-10 02:34:22.000000 PFlowC-2.1.1/PFlowC/geo_proxy.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     7872 2024-04-29 09:28:01.000000 PFlowC-2.1.1/PFlowC/main.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      722 2024-04-28 09:32:05.000000 PFlowC-2.1.1/PFlowC/proxy.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 02:56:49.235808 PFlowC-2.1.1/PFlowC/proxy_helper/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      859 2024-04-29 09:50:09.000000 PFlowC-2.1.1/PFlowC/proxy_helper/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     7391 2024-04-29 09:49:45.000000 PFlowC-2.1.1/PFlowC/proxy_helper/macosx.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 02:56:49.258350 PFlowC-2.1.1/PFlowC/utils/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)  6381855 2024-04-29 05:46:08.000000 PFlowC-2.1.1/PFlowC/utils/Country.mmdb
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-2.1.1/PFlowC/utils/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-2.1.1/PFlowC/utils/logger.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     2000 2024-04-30 09:01:33.000000 PFlowC-2.1.1/PFlowC/utils/net.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 02:56:49.235346 PFlowC-2.1.1/PFlowC.egg-info/
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     2885 2024-05-10 02:56:48.000000 PFlowC-2.1.1/PFlowC.egg-info/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      617 2024-05-10 02:56:48.000000 PFlowC-2.1.1/PFlowC.egg-info/SOURCES.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-05-10 02:56:48.000000 PFlowC-2.1.1/PFlowC.egg-info/dependency_links.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-05-10 02:56:48.000000 PFlowC-2.1.1/PFlowC.egg-info/entry_points.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       64 2024-05-10 02:56:48.000000 PFlowC-2.1.1/PFlowC.egg-info/requires.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-05-10 02:56:48.000000 PFlowC-2.1.1/PFlowC.egg-info/top_level.txt
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     2885 2024-05-10 02:56:49.261629 PFlowC-2.1.1/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1831 2024-05-10 02:51:21.000000 PFlowC-2.1.1/README.rst
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-05-10 02:56:49.261911 PFlowC-2.1.1/setup.cfg
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1778 2024-05-10 02:54:38.000000 PFlowC-2.1.1/setup.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 02:56:49.261054 PFlowC-2.1.1/tests/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3532 2024-04-29 07:46:42.000000 PFlowC-2.1.1/tests/test-agent-service.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      416 2024-04-29 02:59:48.000000 PFlowC-2.1.1/tests/test-api.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      765 2024-04-28 10:17:38.000000 PFlowC-2.1.1/tests/test-banner.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      824 2024-04-30 04:51:51.000000 PFlowC-2.1.1/tests/test-dns-socket.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      858 2024-04-30 08:11:38.000000 PFlowC-2.1.1/tests/test-dnspython.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      532 2024-05-10 02:34:13.000000 PFlowC-2.1.1/tests/test-filter-domains.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      566 2024-04-29 10:14:26.000000 PFlowC-2.1.1/tests/test-json-dump.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1313 2024-04-30 06:00:45.000000 PFlowC-2.1.1/tests/test-salary.py
```

### Comparing `PFlowC-2.1.0/PFlowC/geo_proxy.py` & `PFlowC-2.1.1/PFlowC/geo_proxy.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.1.0/PFlowC/main.py` & `PFlowC-2.1.1/PFlowC/main.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.1.0/PFlowC/proxy.py` & `PFlowC-2.1.1/PFlowC/proxy.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.1.0/PFlowC/proxy_helper/__init__.py` & `PFlowC-2.1.1/PFlowC/proxy_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.1.0/PFlowC/proxy_helper/macosx.py` & `PFlowC-2.1.1/PFlowC/proxy_helper/macosx.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.1.0/PFlowC/utils/Country.mmdb` & `PFlowC-2.1.1/PFlowC/utils/Country.mmdb`

 * *Files identical despite different names*

### Comparing `PFlowC-2.1.0/PFlowC/utils/logger.py` & `PFlowC-2.1.1/PFlowC/utils/logger.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.1.0/PFlowC/utils/net.py` & `PFlowC-2.1.1/PFlowC/utils/net.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.1.0/PFlowC.egg-info/PKG-INFO` & `PFlowC-2.1.1/PFlowC.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 2.1.0
+Version: 2.1.1
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,17 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
 Requires-Dist: colorlog
 Requires-Dist: click
+Requires-Dist: mitmproxy>=10.3.0
+Requires-Dist: geoip2>=4.8.0
+Requires-Dist: dnspython>=2.6.1
 
 FlowPilot ~ PFC ~ Proxy Flow Control
 ========================================================
 
 ProxyFlow Control
 ------------------------------
 
@@ -38,15 +41,15 @@
     ██╔══██╗██╔════╝██║     ██╔═══██╗██║    ██║██╔════╝
     ██████╔╝█████╗  ██║     ██║   ██║██║ █╗ ██║██║
     ██╔═══╝ ██╔══╝  ██║     ██║   ██║██║███╗██║██║
     ██║     ██║     ███████╗╚██████╔╝╚███╔███╔╝╚██████╗
     ╚═╝     ╚═╝     ╚══════╝ ╚═════╝  ╚══╝╚══╝  ╚═════╝
 
     Command line interface for Proxy Flow Controller with basic auto configurations.
-    Version: 2.1.0                    By: BlackHaoke<Haoke98@outlook.com>
+    Version: 2.1.1                    By: BlackHaoke<Haoke98@outlook.com>
     Usage: pflow-cli [OPTIONS] COMMAND [ARGS]...
 
     Options:
       --help  Show this message and exit.
 
     Commands:
       off      Set off and clear all proxy config.
```

### Comparing `PFlowC-2.1.0/PFlowC.egg-info/SOURCES.txt` & `PFlowC-2.1.1/PFlowC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PFlowC-2.1.0/PKG-INFO` & `PFlowC-2.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 2.1.0
+Version: 2.1.1
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,17 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
 Requires-Dist: colorlog
 Requires-Dist: click
+Requires-Dist: mitmproxy>=10.3.0
+Requires-Dist: geoip2>=4.8.0
+Requires-Dist: dnspython>=2.6.1
 
 FlowPilot ~ PFC ~ Proxy Flow Control
 ========================================================
 
 ProxyFlow Control
 ------------------------------
 
@@ -38,15 +41,15 @@
     ██╔══██╗██╔════╝██║     ██╔═══██╗██║    ██║██╔════╝
     ██████╔╝█████╗  ██║     ██║   ██║██║ █╗ ██║██║
     ██╔═══╝ ██╔══╝  ██║     ██║   ██║██║███╗██║██║
     ██║     ██║     ███████╗╚██████╔╝╚███╔███╔╝╚██████╗
     ╚═╝     ╚═╝     ╚══════╝ ╚═════╝  ╚══╝╚══╝  ╚═════╝
 
     Command line interface for Proxy Flow Controller with basic auto configurations.
-    Version: 2.1.0                    By: BlackHaoke<Haoke98@outlook.com>
+    Version: 2.1.1                    By: BlackHaoke<Haoke98@outlook.com>
     Usage: pflow-cli [OPTIONS] COMMAND [ARGS]...
 
     Options:
       --help  Show this message and exit.
 
     Commands:
       off      Set off and clear all proxy config.
```

### Comparing `PFlowC-2.1.0/README.rst` & `PFlowC-2.1.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     ██╔══██╗██╔════╝██║     ██╔═══██╗██║    ██║██╔════╝
     ██████╔╝█████╗  ██║     ██║   ██║██║ █╗ ██║██║
     ██╔═══╝ ██╔══╝  ██║     ██║   ██║██║███╗██║██║
     ██║     ██║     ███████╗╚██████╔╝╚███╔███╔╝╚██████╗
     ╚═╝     ╚═╝     ╚══════╝ ╚═════╝  ╚══╝╚══╝  ╚═════╝
 
     Command line interface for Proxy Flow Controller with basic auto configurations.
-    Version: 2.1.0                    By: BlackHaoke<Haoke98@outlook.com>
+    Version: 2.1.1                    By: BlackHaoke<Haoke98@outlook.com>
     Usage: pflow-cli [OPTIONS] COMMAND [ARGS]...
 
     Options:
       --help  Show this message and exit.
 
     Commands:
       off      Set off and clear all proxy config.
```

### Comparing `PFlowC-2.1.0/setup.py` & `PFlowC-2.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 except ImportError:
     from distutils.core import setup
 
 long_description = open('README.rst', encoding='utf-8').read()
 
 setup(
     name='PFlowC',
-    version='2.1.0',
+    version='2.1.1',
     url='https://github.com/Haoke98/FlowPilot',
     author='Haoke98',
     author_email='BlackHaoke<Haoke98@outlook.com>',
     license='MIT',
     description='https://github.com/Haoke98/FlowPilot/README.md',
     packages=["PFlowC", "PFlowC.utils", "PFlowC.proxy_helper"],
-    install_requires=['colorlog', 'click'],
+    install_requires=['colorlog', 'click', 'mitmproxy>=10.3.0', 'geoip2>=4.8.0', 'dnspython>=2.6.1'],
     package_data={
         'PFlowC.utils': ['Country.mmdb'],
     },
     include_package_data=True,
     python_requires='>=3.7',
     long_description=long_description,
     classifiers=[
```

### Comparing `PFlowC-2.1.0/tests/test-agent-service.py` & `PFlowC-2.1.1/tests/test-agent-service.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.1.0/tests/test-banner.py` & `PFlowC-2.1.1/tests/test-banner.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.1.0/tests/test-dns-socket.py` & `PFlowC-2.1.1/tests/test-dns-socket.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.1.0/tests/test-dnspython.py` & `PFlowC-2.1.1/tests/test-dnspython.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.1.0/tests/test-filter-domains.py` & `PFlowC-2.1.1/tests/test-filter-domains.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.1.0/tests/test-json-dump.py` & `PFlowC-2.1.1/tests/test-json-dump.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.1.0/tests/test-salary.py` & `PFlowC-2.1.1/tests/test-salary.py`

 * *Files identical despite different names*

