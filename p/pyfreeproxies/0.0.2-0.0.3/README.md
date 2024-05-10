# Comparing `tmp/pyfreeproxies-0.0.2.tar.gz` & `tmp/pyfreeproxies-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfreeproxies-0.0.2.tar", last modified: Fri May 10 02:35:53 2024, max compression
+gzip compressed data, was "pyfreeproxies-0.0.3.tar", last modified: Fri May 10 11:45:17 2024, max compression
```

## Comparing `pyfreeproxies-0.0.2.tar` & `pyfreeproxies-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-10 02:35:53.666883 pyfreeproxies-0.0.2/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)    35149 2024-05-09 22:08:33.000000 pyfreeproxies-0.0.2/LICENSE
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4573 2024-05-10 02:35:53.666883 pyfreeproxies-0.0.2/PKG-INFO
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     3141 2024-05-10 01:58:54.000000 pyfreeproxies-0.0.2/README.md
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       38 2024-05-10 02:35:53.666883 pyfreeproxies-0.0.2/setup.cfg
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2155 2024-05-10 02:32:53.000000 pyfreeproxies-0.0.2/setup.py
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-10 02:35:53.660216 pyfreeproxies-0.0.2/src/
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-10 02:35:53.663549 pyfreeproxies-0.0.2/src/pyfreeproxies/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)      200 2024-05-10 00:10:07.000000 pyfreeproxies-0.0.2/src/pyfreeproxies/__init__.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)      767 2024-05-10 00:40:58.000000 pyfreeproxies-0.0.2/src/pyfreeproxies/models.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4914 2024-05-10 01:21:18.000000 pyfreeproxies-0.0.2/src/pyfreeproxies/proxies.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     1886 2024-05-10 01:58:09.000000 pyfreeproxies-0.0.2/src/pyfreeproxies/utils.py
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-10 02:35:53.666883 pyfreeproxies-0.0.2/src/pyfreeproxies.egg-info/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4573 2024-05-10 02:35:53.000000 pyfreeproxies-0.0.2/src/pyfreeproxies.egg-info/PKG-INFO
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)      414 2024-05-10 02:35:53.000000 pyfreeproxies-0.0.2/src/pyfreeproxies.egg-info/SOURCES.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)        1 2024-05-10 02:35:53.000000 pyfreeproxies-0.0.2/src/pyfreeproxies.egg-info/dependency_links.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       47 2024-05-10 02:35:53.000000 pyfreeproxies-0.0.2/src/pyfreeproxies.egg-info/entry_points.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       33 2024-05-10 02:35:53.000000 pyfreeproxies-0.0.2/src/pyfreeproxies.egg-info/requires.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       14 2024-05-10 02:35:53.000000 pyfreeproxies-0.0.2/src/pyfreeproxies.egg-info/top_level.txt
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-10 02:35:53.666883 pyfreeproxies-0.0.2/tests/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2117 2024-05-10 01:19:39.000000 pyfreeproxies-0.0.2/tests/test_freeproxies.py
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-10 11:45:17.029023 pyfreeproxies-0.0.3/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    35149 2024-05-09 22:08:33.000000 pyfreeproxies-0.0.3/LICENSE
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4573 2024-05-10 11:45:17.029023 pyfreeproxies-0.0.3/PKG-INFO
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     3141 2024-05-10 01:58:54.000000 pyfreeproxies-0.0.3/README.md
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       38 2024-05-10 11:45:17.029023 pyfreeproxies-0.0.3/setup.cfg
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2155 2024-05-10 11:43:07.000000 pyfreeproxies-0.0.3/setup.py
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-10 11:45:17.012356 pyfreeproxies-0.0.3/src/
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-10 11:45:17.022356 pyfreeproxies-0.0.3/src/pyfreeproxies/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      200 2024-05-10 00:10:07.000000 pyfreeproxies-0.0.3/src/pyfreeproxies/__init__.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      767 2024-05-10 00:40:58.000000 pyfreeproxies-0.0.3/src/pyfreeproxies/models.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4914 2024-05-10 01:21:18.000000 pyfreeproxies-0.0.3/src/pyfreeproxies/proxies.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     1886 2024-05-10 01:58:09.000000 pyfreeproxies-0.0.3/src/pyfreeproxies/utils.py
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-10 11:45:17.029023 pyfreeproxies-0.0.3/src/pyfreeproxies.egg-info/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4573 2024-05-10 11:45:16.000000 pyfreeproxies-0.0.3/src/pyfreeproxies.egg-info/PKG-INFO
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      414 2024-05-10 11:45:16.000000 pyfreeproxies-0.0.3/src/pyfreeproxies.egg-info/SOURCES.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)        1 2024-05-10 11:45:16.000000 pyfreeproxies-0.0.3/src/pyfreeproxies.egg-info/dependency_links.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       47 2024-05-10 11:45:16.000000 pyfreeproxies-0.0.3/src/pyfreeproxies.egg-info/entry_points.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       33 2024-05-10 11:45:16.000000 pyfreeproxies-0.0.3/src/pyfreeproxies.egg-info/requires.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       14 2024-05-10 11:45:16.000000 pyfreeproxies-0.0.3/src/pyfreeproxies.egg-info/top_level.txt
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-10 11:45:17.025689 pyfreeproxies-0.0.3/tests/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2117 2024-05-10 01:19:39.000000 pyfreeproxies-0.0.3/tests/test_freeproxies.py
```

### Comparing `pyfreeproxies-0.0.2/LICENSE` & `pyfreeproxies-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfreeproxies-0.0.2/PKG-INFO` & `pyfreeproxies-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfreeproxies
-Version: 0.0.2
+Version: 0.0.3
 Summary: Free to use http, socks4 and socks5 proxies
 Home-page: https://github.com/Simatwa/pyfreeproxies
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: GNUv3
 Project-URL: Bug Report, https://github.com/Simatwa/pyfreeproxies/issues/new
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyfreeproxies Version: 0.0.2 Summary: Free to use
+Metadata-Version: 2.1 Name: pyfreeproxies Version: 0.0.3 Summary: Free to use
 http, socks4 and socks5 proxies Home-page: https://github.com/Simatwa/
 pyfreeproxies Author: Smartwa Author-email: simatwacaleb@proton.me Maintainer:
 Smartwa License: GNUv3 Project-URL: Bug Report, https://github.com/Simatwa/
 pyfreeproxies/issues/new Project-URL: Homepage, https://github.com/Simatwa/
 pyfreeproxies Project-URL: Source Code, https://github.com/Simatwa/
 pyfreeproxies Project-URL: Issue Tracker, https://github.com/Simatwa/
 pyfreeproxies/issues Project-URL: Download, https://github.com/Simatwa/
```

### Comparing `pyfreeproxies-0.0.2/README.md` & `pyfreeproxies-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyfreeproxies-0.0.2/setup.py` & `pyfreeproxies-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="pyfreeproxies",
-    version="0.0.2",
+    version="0.0.3",
     license="GNUv3",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Free to use http, socks4 and socks5 proxies",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `pyfreeproxies-0.0.2/src/pyfreeproxies/models.py` & `pyfreeproxies-0.0.3/src/pyfreeproxies/models.py`

 * *Files identical despite different names*

### Comparing `pyfreeproxies-0.0.2/src/pyfreeproxies/proxies.py` & `pyfreeproxies-0.0.3/src/pyfreeproxies/proxies.py`

 * *Files identical despite different names*

### Comparing `pyfreeproxies-0.0.2/src/pyfreeproxies/utils.py` & `pyfreeproxies-0.0.3/src/pyfreeproxies/utils.py`

 * *Files identical despite different names*

### Comparing `pyfreeproxies-0.0.2/src/pyfreeproxies.egg-info/PKG-INFO` & `pyfreeproxies-0.0.3/src/pyfreeproxies.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfreeproxies
-Version: 0.0.2
+Version: 0.0.3
 Summary: Free to use http, socks4 and socks5 proxies
 Home-page: https://github.com/Simatwa/pyfreeproxies
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: GNUv3
 Project-URL: Bug Report, https://github.com/Simatwa/pyfreeproxies/issues/new
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyfreeproxies Version: 0.0.2 Summary: Free to use
+Metadata-Version: 2.1 Name: pyfreeproxies Version: 0.0.3 Summary: Free to use
 http, socks4 and socks5 proxies Home-page: https://github.com/Simatwa/
 pyfreeproxies Author: Smartwa Author-email: simatwacaleb@proton.me Maintainer:
 Smartwa License: GNUv3 Project-URL: Bug Report, https://github.com/Simatwa/
 pyfreeproxies/issues/new Project-URL: Homepage, https://github.com/Simatwa/
 pyfreeproxies Project-URL: Source Code, https://github.com/Simatwa/
 pyfreeproxies Project-URL: Issue Tracker, https://github.com/Simatwa/
 pyfreeproxies/issues Project-URL: Download, https://github.com/Simatwa/
```

### Comparing `pyfreeproxies-0.0.2/tests/test_freeproxies.py` & `pyfreeproxies-0.0.3/tests/test_freeproxies.py`

 * *Files identical despite different names*

