# Comparing `tmp/ansar_connect-0.1.239.tar.gz` & `tmp/ansar_connect-0.1.240.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.239.tar", last modified: Thu May  9 13:47:41 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.240.tar", last modified: Fri May 10 01:08:50 2024, max compression
```

## Comparing `ansar_connect-0.1.239.tar` & `ansar_connect-0.1.240.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:47:41.440827 ansar_connect-0.1.239/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.239/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-09 13:47:41.440827 ansar_connect-0.1.239/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.239/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-09 12:39:56.000000 ansar_connect-0.1.239/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-09 13:47:41.440827 ansar_connect-0.1.239/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-09 12:39:45.000000 ansar_connect-0.1.239/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:47:41.436827 ansar_connect-0.1.239/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:47:41.436827 ansar_connect-0.1.239/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:47:41.436827 ansar_connect-0.1.239/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.239/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3259 2024-05-08 21:30:23.000000 ansar_connect-0.1.239/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.239/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8855 2024-05-08 21:32:04.000000 ansar_connect-0.1.239/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:47:41.436827 ansar_connect-0.1.239/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-09 13:47:38.000000 ansar_connect-0.1.239/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.239/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    87458 2024-05-09 02:23:09.000000 ansar_connect-0.1.239/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.239/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.239/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.239/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14241 2024-05-09 13:41:02.000000 ansar_connect-0.1.239/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.239/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.239/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.239/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8453 2024-05-09 12:04:12.000000 ansar_connect-0.1.239/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.239/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.239/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.239/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    38992 2024-05-09 00:38:31.000000 ansar_connect-0.1.239/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.239/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.239/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.239/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.239/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:47:41.440827 ansar_connect-0.1.239/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-09 13:47:41.000000 ansar_connect-0.1.239/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-09 13:47:41.000000 ansar_connect-0.1.239/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-09 13:47:41.000000 ansar_connect-0.1.239/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-09 13:47:41.000000 ansar_connect-0.1.239/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-09 13:47:41.000000 ansar_connect-0.1.239/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-09 13:47:41.000000 ansar_connect-0.1.239/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-10 01:08:50.650028 ansar_connect-0.1.240/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.240/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-10 01:08:50.650028 ansar_connect-0.1.240/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.240/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-09 12:39:56.000000 ansar_connect-0.1.240/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-10 01:08:50.650028 ansar_connect-0.1.240/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-09 12:39:45.000000 ansar_connect-0.1.240/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-10 01:08:50.646028 ansar_connect-0.1.240/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-10 01:08:50.646028 ansar_connect-0.1.240/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-10 01:08:50.650028 ansar_connect-0.1.240/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.240/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3259 2024-05-08 21:30:23.000000 ansar_connect-0.1.240/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.240/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8855 2024-05-08 21:32:04.000000 ansar_connect-0.1.240/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-10 01:08:50.650028 ansar_connect-0.1.240/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-10 01:08:47.000000 ansar_connect-0.1.240/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.240/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    87458 2024-05-09 02:23:09.000000 ansar_connect-0.1.240/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.240/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10470 2024-05-10 00:12:45.000000 ansar_connect-0.1.240/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.240/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14241 2024-05-09 13:41:02.000000 ansar_connect-0.1.240/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.240/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.240/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.240/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8453 2024-05-09 12:04:12.000000 ansar_connect-0.1.240/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.240/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33939 2024-05-10 00:17:44.000000 ansar_connect-0.1.240/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.240/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38992 2024-05-09 00:38:31.000000 ansar_connect-0.1.240/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.240/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.240/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.240/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.240/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-10 01:08:50.650028 ansar_connect-0.1.240/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-10 01:08:50.000000 ansar_connect-0.1.240/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-10 01:08:50.000000 ansar_connect-0.1.240/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-10 01:08:50.000000 ansar_connect-0.1.240/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-10 01:08:50.000000 ansar_connect-0.1.240/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-10 01:08:50.000000 ansar_connect-0.1.240/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-10 01:08:50.000000 ansar_connect-0.1.240/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.239/LICENSE` & `ansar_connect-0.1.240/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/PKG-INFO` & `ansar_connect-0.1.240/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.239
+Version: 0.1.240
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.239/README.md` & `ansar_connect-0.1.240/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/pyproject.toml` & `ansar_connect-0.1.240/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/setup.py` & `ansar_connect-0.1.240/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.240/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.240/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.240/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.240/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/connect/__init__.py` & `ansar_connect-0.1.240/src/ansar/connect/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 87e3d79e1f2cf3c6bd9fb977a6e7533e98f2c6aa
-Version: 0.1.238 (2024-05-10@01:47:38+NZST)
+Commit: daccac243e99544a0b85e650625daae805371162
+Version: 0.1.239 (2024-05-10@13:08:47+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.239/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.240/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/connect/directory.py` & `ansar_connect-0.1.240/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.240/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.240/src/ansar/connect/foh_if.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,17 @@
 	'FOH_PORT',
 	'AccountSignup',
 	'AccountLogin',
 	'AccountRead',
 	'AccountUpdate',
 	'AccountDelete',
 	'AccountAddLogin',
+	'AccountDeleteLogin',
 	'AccountAddDirectory',
+	'AccountDeleteDirectory',
 	'LoginRead',
 	'DirectoryRead',
 	'DirectoryUpdate',
 	'DirectoryExport',
 	'AccountOpened',
 	'DirectoryExported',
 	'DirectoryPage',
@@ -96,21 +98,31 @@
 		self.login_email = login_email
 		self.password = password
 		self.family_name = family_name
 		self.given_name = given_name
 		self.nick_name = nick_name
 		self.honorific = honorific
 
+class AccountDeleteLogin(object):
+	def __init__(self, login_token=None, login_email=None):
+		self.login_token = login_token
+		self.login_email = login_email
+
 class AccountAddDirectory(object):
 	def __init__(self, login_token=None,
 			product_name=None, product_instance=None):
 		self.login_token = login_token
 		self.product_name = product_name
 		self.product_instance = product_instance
 
+class AccountDeleteDirectory(object):
+	def __init__(self, login_token=None, directory_id=None):
+		self.login_token = login_token
+		self.directory_id = directory_id
+
 class LoginRead(object):
 	def __init__(self, login_token=None):
 		self.login_token = login_token
 
 class DirectoryRead(object):
 	def __init__(self, login_token=None, directory_id=None):
 		self.login_token = login_token
@@ -164,15 +176,17 @@
 
 ar.bind(AccountSignup, object_schema=SHARED_SCHEMA)
 ar.bind(AccountLogin, object_schema=SHARED_SCHEMA)
 ar.bind(AccountRead, object_schema=SHARED_SCHEMA)
 ar.bind(AccountUpdate, object_schema=SHARED_SCHEMA)
 ar.bind(AccountDelete, object_schema=SHARED_SCHEMA)
 ar.bind(AccountAddLogin, object_schema=SHARED_SCHEMA)
+ar.bind(AccountDeleteLogin, object_schema=SHARED_SCHEMA)
 ar.bind(AccountAddDirectory, object_schema=SHARED_SCHEMA)
+ar.bind(AccountDeleteDirectory, object_schema=SHARED_SCHEMA)
 ar.bind(LoginRead, object_schema=SHARED_SCHEMA)
 ar.bind(DirectoryRead, object_schema=SHARED_SCHEMA)
 ar.bind(DirectoryUpdate, object_schema=SHARED_SCHEMA)
 ar.bind(DirectoryExport, object_schema=SHARED_SCHEMA)
 
 # Forms and responses to present to cloud clients.
 class AccountOpened(object):
```

### Comparing `ansar_connect-0.1.239/src/ansar/connect/group_if.py` & `ansar_connect-0.1.240/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/connect/grouping.py` & `ansar_connect-0.1.240/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/connect/moving.py` & `ansar_connect-0.1.240/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/connect/networking.py` & `ansar_connect-0.1.240/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.240/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/connect/node.py` & `ansar_connect-0.1.240/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.240/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/connect/procedure.py` & `ansar_connect-0.1.240/src/ansar/connect/procedure.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 import os
 import getpass
 import uuid
 import ansar.connect as ar
 from ansar.encode.args import QUOTED_TYPE, SHIPMENT_WITH_QUOTES, SHIPMENT_WITHOUT_QUOTES
 from ansar.create.procedure import DEFAULT_HOME, DEFAULT_GROUP, HOME, GROUP
 from ansar.create.procedure import open_home, role_status
-from ansar.create.object import decoration_store
+from ansar.create.object import decoration_store, object_settings
 from ansar.connect.group_if import GroupSettings
 from ansar.connect.standard import *
 from .foh_if import *
 from .wan import *
 from .product import *
 from .directory_if import *
 
@@ -462,33 +462,39 @@
 			continue
 		d = fill_field(k, v)
 		setattr(form, k, d)
 
 #
 #
 class AccountSettings(object):
-	def __init__(self, read=False, update=False, delete=False, add_login=False, add_directory=False,
+	def __init__(self, read=False, update=False, delete=False,
+			add_login=False, delete_login=False,
+			add_directory=False, delete_directory=False,
 			organization_name=None, organization_location=None,
 			show_identities=False, show_times=False):
 		self.read = read
 		self.update = update
 		self.delete = delete
 		self.add_login = add_login
+		self.delete_login = delete_login
 		self.add_directory = add_directory
+		self.delete_directory = delete_directory
 		self.organization_name = organization_name
 		self.organization_location = organization_location
 		self.show_identities = show_identities
 		self.show_times = show_times
 
 ACCOUNT_SETTINGS_SCHEMA = {
 	'read': ar.Boolean(),
 	'update': ar.Boolean(),
 	'delete': ar.Boolean(),
 	'add_login': ar.Boolean(),
+	'delete_login': ar.Boolean(),
 	'add_directory': ar.Boolean(),
+	'delete_directory': ar.Boolean(),
 	'organization_name': ar.Unicode(),
 	'organization_location': ar.Unicode(),
 	'show_identities': ar.Boolean(),
 	'show_times': ar.Boolean(),
 }
 
 ar.bind(AccountSettings, object_schema=ACCOUNT_SETTINGS_SCHEMA)
@@ -580,15 +586,17 @@
 # CRUD for the account entity. Well, more like RUD as
 # the create part is covered by signup and login.
 def procedure_account(self, account):
 	settings = ar.object_custom_settings()
 	cloud_ip = settings.cloud_ip
 	login_token = settings.login_token
 
-	crud = sum([account.read, account.update, account.delete, account.add_login, account.add_directory])
+	crud = sum([account.read, account.update, account.delete,
+		account.add_login, account.delete_login,
+		account.add_directory, account.delete_directory])
 
 	f = crud_address_and_token(crud, cloud_ip, login_token)
 	if f:
 		return f
 
 	encrypted = settings.encrypted
 	ar.connect(self, ar.HostPort(cloud_ip, FOH_PORT), encrypted=encrypted)
@@ -603,16 +611,20 @@
 	try:
 		if account.update:
 			return account_update(self, login_token, session, account)
 		elif account.delete:
 			return account_delete(self, login_token, session)
 		elif account.add_login:
 			return account_add_login(self, login_token, session)
+		elif account.delete_login:
+			return account_delete_login(self, login_token, session)
 		elif account.add_directory:
 			return account_add_directory(self, login_token, session)
+		elif account.delete_directory:
+			return account_delete_directory(self, login_token, session)
 		return account_read(self, login_token, session, account)
 	finally:
 		self.send(ar.Close(), session)
 		self.select(ar.Closed, ar.Stop)
 
 def account_signup(self, session):
 	signup = AccountSignup()
@@ -634,44 +646,40 @@
 	ar.store_settings(settings)
 	return None
 
 def account_login(self, session):
 	login = AccountLogin()
 	fill_form(self, login)
 	self.send(login, session)
-	m = self.select(AccountOpened, ar.Faulted, ar.Abandoned, ar.Stop)
+	m = self.select(AccountOpened, ar.Faulted, ar.Closed, ar.Abandoned, ar.Stop)
 	if isinstance(m, AccountOpened):
 		pass
 	elif isinstance(m, ar.Faulted):
 		return m
-	elif isinstance(m, ar.Abandoned):
-		f = ar.Faulted('remote abandoned connection', 'try later?')
-		return f
+	elif isinstance(m, (ar.Closed, ar.Abandoned)):
+		return m
 	else:
 		return ar.Aborted()
 
 	settings = ar.object_custom_settings()
 	settings.login_token = m.login_token
 	ar.store_settings(settings)
 	return None
 
 def account_read(self, login_token, session, account):
 	read = AccountRead(login_token=login_token)
 	self.send(read, session)
 	m = self.select(AccountPage, ar.Faulted, ar.Abandoned, ar.Closed, ar.Stop)
 	if isinstance(m, AccountPage):
-		output_account(m, account)
-	elif isinstance(m, ar.Faulted):
-		return m
-	elif isinstance(m, (ar.Abandoned, ar.Closed)):
-		f = ar.Faulted('lost remote connection', 'try later?')
-		return f
-	else:
-		return ar.Aborted()
-	return None
+		if not object_settings.pure_object:
+			output_account(m, account)
+			return None
+	elif isinstance(m, ar.Stop):
+		m = ar.Aborted()
+	return m
 
 def account_update(self, login_token, session, account):
 	update = AccountUpdate(login_token=login_token,
 		organization_name=account.organization_name, organization_location=account.organization_location)
 
 	if not account.organization_name and not account.organization_location:
 		fill_form(self, update)
@@ -709,16 +717,30 @@
 	self.send(add, session)
 	m = self.select(LoginPage, ar.Faulted, ar.Abandoned, ar.Stop)
 	if isinstance(m, LoginPage):
 		pass
 	elif isinstance(m, ar.Faulted):
 		return m
 	elif isinstance(m, ar.Abandoned):
-		f = ar.Faulted('remote abandoned connection', 'try later?')
-		return f
+		return m
+	else:
+		return ar.Aborted()
+	return None
+
+def account_delete_login(self, login_token, session):
+	delete = AccountDeleteLogin(login_token=login_token)
+	fill_form(self, delete)
+	self.send(delete, session)
+	m = self.select(LoginDeleted, ar.Faulted, ar.Abandoned, ar.Stop)
+	if isinstance(m, LoginDeleted):
+		pass
+	elif isinstance(m, ar.Faulted):
+		return m
+	elif isinstance(m, ar.Abandoned):
+		return m
 	else:
 		return ar.Aborted()
 	return None
 
 def account_add_directory(self, login_token, session):
 	add = AccountAddDirectory(login_token=login_token)
 	fill_form(self, add)
@@ -731,14 +753,30 @@
 	elif isinstance(m, ar.Abandoned):
 		f = ar.Faulted('remote abandoned connection', 'try later?')
 		return f
 	else:
 		return ar.Aborted()
 	return None
 
+def account_delete_directory(self, login_token, session):
+	delete = AccountDeleteDirectory(login_token=login_token)
+	fill_form(self, delete)
+	self.send(delete, session)
+	m = self.select(DirectoryDeleted, ar.Faulted, ar.Abandoned, ar.Stop)
+	if isinstance(m, DirectoryDeleted):
+		pass
+	elif isinstance(m, ar.Faulted):
+		return m
+	elif isinstance(m, ar.Abandoned):
+		return m
+	else:
+		return ar.Aborted()
+	return None
+
+
 '''		self.account_id = account_id				# Unique key.
 		self.organization_name = organization_name
 		self.organization_location = organization_location
 		self.technical_contact = technical_contact or ar.default_vector()
 		self.financial_contact = financial_contact or ar.default_vector()
 		self.administrative_contact = administrative_contact or ar.default_vector()
 		self.number_of_logins = number_of_logins
```

### Comparing `ansar_connect-0.1.239/src/ansar/connect/product.py` & `ansar_connect-0.1.240/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/connect/socketry.py` & `ansar_connect-0.1.240/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/connect/standard.py` & `ansar_connect-0.1.240/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/connect/transporting.py` & `ansar_connect-0.1.240/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.240/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar/connect/wan.py` & `ansar_connect-0.1.240/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.239/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.240/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.239
+Version: 0.1.240
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.239/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.240/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

