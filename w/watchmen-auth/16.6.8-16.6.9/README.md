# Comparing `tmp/watchmen_auth-16.6.8.tar.gz` & `tmp/watchmen_auth-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_auth-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_auth-16.6.9.tar", max compression
```

## Comparing `watchmen_auth-16.6.8.tar` & `watchmen_auth-16.6.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.488594 watchmen_auth-16.6.8/LICENSE
--rw-r--r--   0        0        0      418 2024-01-08 07:58:02.492594 watchmen_auth-16.6.8/pyproject.toml
--rw-r--r--   0        0        0      362 2024-01-08 07:58:02.492594 watchmen_auth-16.6.8/src/watchmen_auth/__init__.py
--rw-r--r--   0        0        0      755 2024-01-08 07:58:02.492594 watchmen_auth-16.6.8/src/watchmen_auth/auth_helper.py
--rw-r--r--   0        0        0     1569 2024-01-08 07:58:02.492594 watchmen_auth-16.6.8/src/watchmen_auth/authentication.py
--rw-r--r--   0        0        0     1212 2024-01-08 07:58:02.492594 watchmen_auth-16.6.8/src/watchmen_auth/authorization.py
--rw-r--r--   0        0        0      742 2024-01-08 07:58:02.492594 watchmen_auth-16.6.8/src/watchmen_auth/fake_principal_service.py
--rw-r--r--   0        0        0      816 2024-01-08 07:58:02.492594 watchmen_auth-16.6.8/src/watchmen_auth/principal_service.py
--rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 watchmen_auth-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.223322 watchmen_auth-16.6.9/LICENSE
+-rw-r--r--   0        0        0      418 2024-02-01 01:32:37.227322 watchmen_auth-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0      362 2024-02-01 01:32:37.227322 watchmen_auth-16.6.9/src/watchmen_auth/__init__.py
+-rw-r--r--   0        0        0      755 2024-02-01 01:32:37.227322 watchmen_auth-16.6.9/src/watchmen_auth/auth_helper.py
+-rw-r--r--   0        0        0     1569 2024-02-01 01:32:37.227322 watchmen_auth-16.6.9/src/watchmen_auth/authentication.py
+-rw-r--r--   0        0        0     1212 2024-02-01 01:32:37.227322 watchmen_auth-16.6.9/src/watchmen_auth/authorization.py
+-rw-r--r--   0        0        0      742 2024-02-01 01:32:37.227322 watchmen_auth-16.6.9/src/watchmen_auth/fake_principal_service.py
+-rw-r--r--   0        0        0      816 2024-02-01 01:32:37.227322 watchmen_auth-16.6.9/src/watchmen_auth/principal_service.py
+-rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 watchmen_auth-16.6.9/PKG-INFO
```

### Comparing `watchmen_auth-16.6.8/LICENSE` & `watchmen_auth-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_auth-16.6.8/src/watchmen_auth/auth_helper.py` & `watchmen_auth-16.6.9/src/watchmen_auth/auth_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_auth-16.6.8/src/watchmen_auth/authentication.py` & `watchmen_auth-16.6.9/src/watchmen_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `watchmen_auth-16.6.8/src/watchmen_auth/authorization.py` & `watchmen_auth-16.6.9/src/watchmen_auth/authorization.py`

 * *Files identical despite different names*

### Comparing `watchmen_auth-16.6.8/src/watchmen_auth/fake_principal_service.py` & `watchmen_auth-16.6.9/src/watchmen_auth/fake_principal_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_auth-16.6.8/src/watchmen_auth/principal_service.py` & `watchmen_auth-16.6.9/src/watchmen_auth/principal_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_auth-16.6.8/PKG-INFO` & `watchmen_auth-16.6.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-auth
-Version: 16.6.8
+Version: 16.6.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: watchmen-model (==16.6.8)
+Requires-Dist: watchmen-model (==16.6.9)
```

