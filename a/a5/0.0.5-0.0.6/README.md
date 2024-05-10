# Comparing `tmp/a5-0.0.5.tar.gz` & `tmp/a5-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a5-0.0.5.tar", last modified: Sun May  5 21:50:20 2024, max compression
+gzip compressed data, was "a5-0.0.6.tar", last modified: Fri May 10 18:45:07 2024, max compression
```

## Comparing `a5-0.0.5.tar` & `a5-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 21:50:20.675934 a5-0.0.5/
--rw-r--r--   0 aapeli    (1000) aapeli    (1000)      239 2024-05-05 21:50:20.675934 a5-0.0.5/PKG-INFO
-drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 21:50:20.671934 a5-0.0.5/a5/
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 18:49:21.000000 a5-0.0.5/a5/__init__.py
-drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 21:50:20.671934 a5-0.0.5/a5/grpc/
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 19:16:57.000000 a5-0.0.5/a5/grpc/__init__.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 19:21:13.000000 a5-0.0.5/a5/grpc/reflection_utils.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     3300 2024-05-05 21:49:43.000000 a5-0.0.5/a5/grpc/rpc_utils.py
-drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 21:50:20.671934 a5-0.0.5/a5/security/
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 21:06:01.000000 a5-0.0.5/a5/security/__init__.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     3130 2024-05-05 21:49:43.000000 a5-0.0.5/a5/security/crypto.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        6 2024-05-05 21:49:32.000000 a5-0.0.5/a5/version
-drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 21:50:20.671934 a5-0.0.5/a5/web/
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 18:49:32.000000 a5-0.0.5/a5/web/__init__.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     1394 2024-05-05 21:49:43.000000 a5-0.0.5/a5/web/basic_web_server.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     1399 2024-05-05 18:50:15.000000 a5-0.0.5/a5/web/cookies.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     1752 2024-05-05 18:49:32.000000 a5-0.0.5/a5/web/http_status_codes.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      977 2024-05-05 18:51:04.000000 a5-0.0.5/a5/web/static_file_server.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      937 2024-05-05 18:49:32.000000 a5-0.0.5/a5/web/tiny_web_server.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     3542 2024-05-05 21:49:43.000000 a5-0.0.5/a5/web/tls.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      689 2024-05-05 18:49:32.000000 a5-0.0.5/a5/web/wsgi_server.py
-drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 21:50:20.675934 a5-0.0.5/a5.egg-info/
--rw-r--r--   0 aapeli    (1000) aapeli    (1000)      239 2024-05-05 21:50:20.000000 a5-0.0.5/a5.egg-info/PKG-INFO
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      506 2024-05-05 21:50:20.000000 a5-0.0.5/a5.egg-info/SOURCES.txt
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        1 2024-05-05 21:50:20.000000 a5-0.0.5/a5.egg-info/dependency_links.txt
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)       32 2024-05-05 21:50:20.000000 a5-0.0.5/a5.egg-info/requires.txt
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        3 2024-05-05 21:50:20.000000 a5-0.0.5/a5.egg-info/top_level.txt
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      330 2024-05-05 18:58:17.000000 a5-0.0.5/pyproject.toml
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)       38 2024-05-05 21:50:20.675934 a5-0.0.5/setup.cfg
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      505 2024-05-05 21:07:05.000000 a5-0.0.5/setup.py
+drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-10 18:45:07.485068 a5-0.0.6/
+-rw-r--r--   0 aapeli    (1000) aapeli    (1000)      239 2024-05-10 18:45:07.485068 a5-0.0.6/PKG-INFO
+drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-10 18:45:07.481068 a5-0.0.6/a5/
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)       44 2024-05-10 18:44:10.000000 a5-0.0.6/a5/__init__.py
+drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-10 18:45:07.481068 a5-0.0.6/a5/grpc/
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 19:16:57.000000 a5-0.0.6/a5/grpc/__init__.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 19:21:13.000000 a5-0.0.6/a5/grpc/reflection_utils.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     3351 2024-05-06 14:49:43.000000 a5-0.0.6/a5/grpc/rpc_utils.py
+drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-10 18:45:07.481068 a5-0.0.6/a5/security/
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 21:06:01.000000 a5-0.0.6/a5/security/__init__.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     3130 2024-05-05 21:49:43.000000 a5-0.0.6/a5/security/crypto.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        6 2024-05-10 18:44:17.000000 a5-0.0.6/a5/version
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)       92 2024-05-10 18:44:53.000000 a5-0.0.6/a5/version.py
+drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-10 18:45:07.481068 a5-0.0.6/a5/web/
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        0 2024-05-05 18:49:32.000000 a5-0.0.6/a5/web/__init__.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     1394 2024-05-05 21:49:43.000000 a5-0.0.6/a5/web/basic_web_server.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     1399 2024-05-05 18:50:15.000000 a5-0.0.6/a5/web/cookies.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     1752 2024-05-05 18:49:32.000000 a5-0.0.6/a5/web/http_status_codes.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      977 2024-05-05 18:51:04.000000 a5-0.0.6/a5/web/static_file_server.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      937 2024-05-05 18:49:32.000000 a5-0.0.6/a5/web/tiny_web_server.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     3542 2024-05-05 21:49:43.000000 a5-0.0.6/a5/web/tls.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      689 2024-05-05 18:49:32.000000 a5-0.0.6/a5/web/wsgi_server.py
+drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2024-05-10 18:45:07.485068 a5-0.0.6/a5.egg-info/
+-rw-r--r--   0 aapeli    (1000) aapeli    (1000)      239 2024-05-10 18:45:07.000000 a5-0.0.6/a5.egg-info/PKG-INFO
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      522 2024-05-10 18:45:07.000000 a5-0.0.6/a5.egg-info/SOURCES.txt
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        1 2024-05-10 18:45:07.000000 a5-0.0.6/a5.egg-info/dependency_links.txt
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)       32 2024-05-10 18:45:07.000000 a5-0.0.6/a5.egg-info/requires.txt
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        3 2024-05-10 18:45:07.000000 a5-0.0.6/a5.egg-info/top_level.txt
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      330 2024-05-05 18:58:17.000000 a5-0.0.6/pyproject.toml
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)       38 2024-05-10 18:45:07.485068 a5-0.0.6/setup.cfg
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      505 2024-05-05 21:07:05.000000 a5-0.0.6/setup.py
```

### Comparing `a5-0.0.5/a5/grpc/rpc_utils.py` & `a5-0.0.6/a5/grpc/rpc_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import functools
 from urllib.parse import urlparse
 
 import grpc
 from google.protobuf import descriptor, descriptor_pb2, descriptor_pool, message_factory
 
 
+class DynamicGrpcClient:
+    def __init__(self, )
+
 class CookieAuthPlugin(grpc.AuthMetadataPlugin):
     def __init__(self, cookie):
         self._cookie = cookie
 
     def __call__(self, context, callback):
         callback((("cookie", f"couchers-sesh={self._cookie}"),), None)
```

### Comparing `a5-0.0.5/a5/security/crypto.py` & `a5-0.0.6/a5/security/crypto.py`

 * *Files identical despite different names*

### Comparing `a5-0.0.5/a5/web/basic_web_server.py` & `a5-0.0.6/a5/web/basic_web_server.py`

 * *Files identical despite different names*

### Comparing `a5-0.0.5/a5/web/cookies.py` & `a5-0.0.6/a5/web/cookies.py`

 * *Files identical despite different names*

### Comparing `a5-0.0.5/a5/web/http_status_codes.py` & `a5-0.0.6/a5/web/http_status_codes.py`

 * *Files identical despite different names*

### Comparing `a5-0.0.5/a5/web/static_file_server.py` & `a5-0.0.6/a5/web/static_file_server.py`

 * *Files identical despite different names*

### Comparing `a5-0.0.5/a5/web/tiny_web_server.py` & `a5-0.0.6/a5/web/tiny_web_server.py`

 * *Files identical despite different names*

### Comparing `a5-0.0.5/a5/web/tls.py` & `a5-0.0.6/a5/web/tls.py`

 * *Files identical despite different names*

### Comparing `a5-0.0.5/a5/web/wsgi_server.py` & `a5-0.0.6/a5/web/wsgi_server.py`

 * *Files identical despite different names*

