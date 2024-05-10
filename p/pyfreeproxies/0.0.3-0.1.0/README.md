# Comparing `tmp/pyfreeproxies-0.0.3.tar.gz` & `tmp/pyfreeproxies-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfreeproxies-0.0.3.tar", last modified: Fri May 10 11:45:17 2024, max compression
+gzip compressed data, was "pyfreeproxies-0.1.0.tar", last modified: Fri May 10 13:43:14 2024, max compression
```

## Comparing `pyfreeproxies-0.0.3.tar` & `pyfreeproxies-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-10 11:45:17.029023 pyfreeproxies-0.0.3/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)    35149 2024-05-09 22:08:33.000000 pyfreeproxies-0.0.3/LICENSE
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4573 2024-05-10 11:45:17.029023 pyfreeproxies-0.0.3/PKG-INFO
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     3141 2024-05-10 01:58:54.000000 pyfreeproxies-0.0.3/README.md
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       38 2024-05-10 11:45:17.029023 pyfreeproxies-0.0.3/setup.cfg
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2155 2024-05-10 11:43:07.000000 pyfreeproxies-0.0.3/setup.py
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-10 11:45:17.012356 pyfreeproxies-0.0.3/src/
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-10 11:45:17.022356 pyfreeproxies-0.0.3/src/pyfreeproxies/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)      200 2024-05-10 00:10:07.000000 pyfreeproxies-0.0.3/src/pyfreeproxies/__init__.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)      767 2024-05-10 00:40:58.000000 pyfreeproxies-0.0.3/src/pyfreeproxies/models.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4914 2024-05-10 01:21:18.000000 pyfreeproxies-0.0.3/src/pyfreeproxies/proxies.py
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     1886 2024-05-10 01:58:09.000000 pyfreeproxies-0.0.3/src/pyfreeproxies/utils.py
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-10 11:45:17.029023 pyfreeproxies-0.0.3/src/pyfreeproxies.egg-info/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4573 2024-05-10 11:45:16.000000 pyfreeproxies-0.0.3/src/pyfreeproxies.egg-info/PKG-INFO
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)      414 2024-05-10 11:45:16.000000 pyfreeproxies-0.0.3/src/pyfreeproxies.egg-info/SOURCES.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)        1 2024-05-10 11:45:16.000000 pyfreeproxies-0.0.3/src/pyfreeproxies.egg-info/dependency_links.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       47 2024-05-10 11:45:16.000000 pyfreeproxies-0.0.3/src/pyfreeproxies.egg-info/entry_points.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       33 2024-05-10 11:45:16.000000 pyfreeproxies-0.0.3/src/pyfreeproxies.egg-info/requires.txt
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)       14 2024-05-10 11:45:16.000000 pyfreeproxies-0.0.3/src/pyfreeproxies.egg-info/top_level.txt
-drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-05-10 11:45:17.025689 pyfreeproxies-0.0.3/tests/
--rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2117 2024-05-10 01:19:39.000000 pyfreeproxies-0.0.3/tests/test_freeproxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:43:14.926293 pyfreeproxies-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-10 13:43:07.000000 pyfreeproxies-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-10 13:43:14.922293 pyfreeproxies-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-10 13:43:14.000000 pyfreeproxies-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:43:14.926293 pyfreeproxies-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-10 13:43:07.000000 pyfreeproxies-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:43:14.922293 pyfreeproxies-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:43:14.922293 pyfreeproxies-0.1.0/src/pyfreeproxies/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-10 13:43:07.000000 pyfreeproxies-0.1.0/src/pyfreeproxies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-10 13:43:07.000000 pyfreeproxies-0.1.0/src/pyfreeproxies/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-05-10 13:43:07.000000 pyfreeproxies-0.1.0/src/pyfreeproxies/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-10 13:43:07.000000 pyfreeproxies-0.1.0/src/pyfreeproxies/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:43:14.922293 pyfreeproxies-0.1.0/src/pyfreeproxies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-10 13:43:14.000000 pyfreeproxies-0.1.0/src/pyfreeproxies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-10 13:43:14.000000 pyfreeproxies-0.1.0/src/pyfreeproxies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:43:14.000000 pyfreeproxies-0.1.0/src/pyfreeproxies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 13:43:14.000000 pyfreeproxies-0.1.0/src/pyfreeproxies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-10 13:43:14.000000 pyfreeproxies-0.1.0/src/pyfreeproxies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 13:43:14.000000 pyfreeproxies-0.1.0/src/pyfreeproxies.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:43:14.922293 pyfreeproxies-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-10 13:43:07.000000 pyfreeproxies-0.1.0/tests/test_freeproxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-10 13:43:07.000000 pyfreeproxies-0.1.0/tests/test_updateawarefreeproxies.py
```

### Comparing `pyfreeproxies-0.0.3/LICENSE` & `pyfreeproxies-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfreeproxies-0.0.3/setup.py` & `pyfreeproxies-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="pyfreeproxies",
-    version="0.0.3",
+    version="0.1.0",
     license="GNUv3",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Free to use http, socks4 and socks5 proxies",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `pyfreeproxies-0.0.3/src/pyfreeproxies/models.py` & `pyfreeproxies-0.1.0/src/pyfreeproxies/models.py`

 * *Files identical despite different names*

### Comparing `pyfreeproxies-0.0.3/tests/test_freeproxies.py` & `pyfreeproxies-0.1.0/tests/test_freeproxies.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.assertIsInstance(self.proxy.get_random_proxies(), list)
 
     def test_combined_proxies(self):
         """Combined proxies fetch"""
         self.assertIsInstance(self.proxy.get_combined_proxies(), dict)
 
     def test_proxy_metadata(self):
-        """Proxes' metadata fetch"""
+        """Proxies' metadata fetch"""
         metadata = self.proxy.get_proxies_metadata()
         self.assertTrue(type(metadata) == dict)
         self.assertIsInstance(list(metadata.values())[0], ProxyMetadataModel)
 
     def test_confirmed_working_proxies(self):
         """Confirmed working proxies"""
         filter = {"country": "United States"}
@@ -49,14 +49,14 @@
             assert ip_metadata.country == filter["country"]
 
     def test_proxies_logs_availability(self):
         """Proxies generation logs availability"""
         self.assertIsInstance(self.proxy.get_proxies_generation_logs(), str)
 
     def test_update(self):
-        """Updare FreeProxies"""
+        """Update FreeProxies"""
         new_FreeProxies = self.proxy.update()
         assert hasattr(new_FreeProxies, "update")
 
 
 if __name__ == "__main__":
     unittest.main()
```

