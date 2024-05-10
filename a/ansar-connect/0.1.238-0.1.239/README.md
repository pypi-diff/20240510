# Comparing `tmp/ansar_connect-0.1.238.tar.gz` & `tmp/ansar_connect-0.1.239.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.238.tar", last modified: Thu May  9 13:42:24 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.239.tar", last modified: Thu May  9 13:47:41 2024, max compression
```

## Comparing `ansar_connect-0.1.238.tar` & `ansar_connect-0.1.239.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:42:24.959350 ansar_connect-0.1.238/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.238/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-09 13:42:24.959350 ansar_connect-0.1.238/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.238/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-09 12:39:56.000000 ansar_connect-0.1.238/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-09 13:42:24.959350 ansar_connect-0.1.238/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-09 12:39:45.000000 ansar_connect-0.1.238/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:42:24.955350 ansar_connect-0.1.238/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:42:24.955350 ansar_connect-0.1.238/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:42:24.955350 ansar_connect-0.1.238/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.238/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3259 2024-05-08 21:30:23.000000 ansar_connect-0.1.238/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.238/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8855 2024-05-08 21:32:04.000000 ansar_connect-0.1.238/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:42:24.959350 ansar_connect-0.1.238/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3009 2024-05-09 13:42:21.000000 ansar_connect-0.1.238/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.238/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    87458 2024-05-09 02:23:09.000000 ansar_connect-0.1.238/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.238/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.238/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.238/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14241 2024-05-09 13:41:02.000000 ansar_connect-0.1.238/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.238/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.238/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.238/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8453 2024-05-09 12:04:12.000000 ansar_connect-0.1.238/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.238/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.238/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.238/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    38992 2024-05-09 00:38:31.000000 ansar_connect-0.1.238/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.238/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.238/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.238/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.238/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:42:24.959350 ansar_connect-0.1.238/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-09 13:42:24.000000 ansar_connect-0.1.238/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-09 13:42:24.000000 ansar_connect-0.1.238/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-09 13:42:24.000000 ansar_connect-0.1.238/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-09 13:42:24.000000 ansar_connect-0.1.238/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-09 13:42:24.000000 ansar_connect-0.1.238/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-09 13:42:24.000000 ansar_connect-0.1.238/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:47:41.440827 ansar_connect-0.1.239/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.239/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-09 13:47:41.440827 ansar_connect-0.1.239/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.239/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-09 12:39:56.000000 ansar_connect-0.1.239/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-09 13:47:41.440827 ansar_connect-0.1.239/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-09 12:39:45.000000 ansar_connect-0.1.239/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:47:41.436827 ansar_connect-0.1.239/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:47:41.436827 ansar_connect-0.1.239/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:47:41.436827 ansar_connect-0.1.239/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.239/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3259 2024-05-08 21:30:23.000000 ansar_connect-0.1.239/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.239/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8855 2024-05-08 21:32:04.000000 ansar_connect-0.1.239/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:47:41.436827 ansar_connect-0.1.239/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-09 13:47:38.000000 ansar_connect-0.1.239/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.239/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    87458 2024-05-09 02:23:09.000000 ansar_connect-0.1.239/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.239/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.239/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.239/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14241 2024-05-09 13:41:02.000000 ansar_connect-0.1.239/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.239/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.239/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.239/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8453 2024-05-09 12:04:12.000000 ansar_connect-0.1.239/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.239/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.239/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.239/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38992 2024-05-09 00:38:31.000000 ansar_connect-0.1.239/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.239/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.239/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.239/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.239/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 13:47:41.440827 ansar_connect-0.1.239/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-09 13:47:41.000000 ansar_connect-0.1.239/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-09 13:47:41.000000 ansar_connect-0.1.239/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-09 13:47:41.000000 ansar_connect-0.1.239/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-09 13:47:41.000000 ansar_connect-0.1.239/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-09 13:47:41.000000 ansar_connect-0.1.239/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-09 13:47:41.000000 ansar_connect-0.1.239/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.238/LICENSE` & `ansar_connect-0.1.239/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/PKG-INFO` & `ansar_connect-0.1.239/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.238
+Version: 0.1.239
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.238/README.md` & `ansar_connect-0.1.239/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/pyproject.toml` & `ansar_connect-0.1.239/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/setup.py` & `ansar_connect-0.1.239/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.239/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.239/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.239/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.239/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/__init__.py` & `ansar_connect-0.1.239/src/ansar/connect/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 398a27bf4d1e9fb789739d65d1c371755d42f40b
-Version: 0.1.237 (2024-05-10@01:42:21+NZST)
+Commit: 87e3d79e1f2cf3c6bd9fb977a6e7533e98f2c6aa
+Version: 0.1.238 (2024-05-10@01:47:38+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
 
@@ -56,15 +56,15 @@
 from .directory import publish, subscribe
 from .directory import clear, retract
 from .directory import key_service
 
 from .networking_if import UseAddress, NoAddress, GlareTimer
 from .networking import ConnectToAddress, ListenAtAddress
 from .networking import SubscribeToListing, PublishAListing, SubscribeToSearch
-from .grouping import GroupTable, GroupUpdate, AddressGroup, GroupTimer, Grouping
+from .grouping import GroupTable, GroupUpdate, AddressGroup, GroupTimer, GroupObject
 
 from .node import NodeSettings, node_settings
 from .node import node_passing, sub_node_passing
 from .node import create_node, NodeProperties
 
 from .moving import overlay, mirror
```

### Comparing `ansar_connect-0.1.238/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.239/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/directory.py` & `ansar_connect-0.1.239/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.239/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.239/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/group_if.py` & `ansar_connect-0.1.239/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/grouping.py` & `ansar_connect-0.1.239/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/moving.py` & `ansar_connect-0.1.239/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/networking.py` & `ansar_connect-0.1.239/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.239/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/node.py` & `ansar_connect-0.1.239/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.239/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/procedure.py` & `ansar_connect-0.1.239/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/product.py` & `ansar_connect-0.1.239/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/socketry.py` & `ansar_connect-0.1.239/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/standard.py` & `ansar_connect-0.1.239/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/transporting.py` & `ansar_connect-0.1.239/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.239/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar/connect/wan.py` & `ansar_connect-0.1.239/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.238/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.239/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.238
+Version: 0.1.239
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.238/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.239/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

