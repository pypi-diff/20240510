# Comparing `tmp/pyjava-0.6.8.tar.gz` & `tmp/pyjava-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjava-0.6.8.tar", last modified: Tue Sep 19 00:09:48 2023, max compression
+gzip compressed data, was "pyjava-0.6.9.tar", last modified: Mon Sep 25 08:44:50 2023, max compression
```

## Comparing `pyjava-0.6.8.tar` & `pyjava-0.6.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-19 00:09:48.306370 pyjava-0.6.8/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      597 2023-09-19 00:09:48.306370 pyjava-0.6.8/PKG-INFO
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      448 2023-04-11 04:53:45.000000 pyjava-0.6.8/README.md
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-19 00:09:48.306370 pyjava-0.6.8/pyjava/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2612 2023-04-11 04:53:45.000000 pyjava-0.6.8/pyjava/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-19 00:09:48.306370 pyjava-0.6.8/pyjava/api/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      688 2023-04-11 04:53:45.000000 pyjava-0.6.8/pyjava/api/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16645 2023-09-18 05:38:30.000000 pyjava-0.6.8/pyjava/api/mlsql.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4524 2023-04-11 04:53:45.000000 pyjava-0.6.8/pyjava/api/serve.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-19 00:09:48.306370 pyjava-0.6.8/pyjava/cache/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.8/pyjava/cache/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      489 2023-04-11 04:53:45.000000 pyjava-0.6.8/pyjava/cache/code_cache.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42222 2023-04-11 04:53:45.000000 pyjava-0.6.8/pyjava/cloudpickle.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7048 2023-04-17 05:24:46.000000 pyjava-0.6.8/pyjava/daemon.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-19 00:09:48.306370 pyjava-0.6.8/pyjava/data/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.8/pyjava/data/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1185 2023-04-11 04:53:45.000000 pyjava-0.6.8/pyjava/data/datasource.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-19 00:09:48.306370 pyjava-0.6.8/pyjava/datatype/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.8/pyjava/datatype/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    64554 2023-04-11 04:53:45.000000 pyjava-0.6.8/pyjava/datatype/types.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2190 2023-04-11 04:53:45.000000 pyjava-0.6.8/pyjava/rayfix.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30195 2023-04-11 04:53:45.000000 pyjava-0.6.8/pyjava/serializers.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-19 00:09:48.306370 pyjava-0.6.8/pyjava/storage/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.8/pyjava/storage/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2825 2023-04-24 06:01:20.000000 pyjava-0.6.8/pyjava/storage/streaming_tar.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-19 00:09:48.306370 pyjava-0.6.8/pyjava/udf/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10721 2023-09-18 16:30:35.000000 pyjava-0.6.8/pyjava/udf/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1555 2023-06-24 13:03:57.000000 pyjava-0.6.8/pyjava/udf/store.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3990 2023-06-23 13:03:45.000000 pyjava-0.6.8/pyjava/utils.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      828 2023-09-19 00:09:38.000000 pyjava-0.6.8/pyjava/version.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6457 2023-04-18 03:10:44.000000 pyjava-0.6.8/pyjava/worker.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-19 00:09:48.306370 pyjava-0.6.8/pyjava.egg-info/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      597 2023-09-19 00:09:48.000000 pyjava-0.6.8/pyjava.egg-info/PKG-INFO
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      616 2023-09-19 00:09:48.000000 pyjava-0.6.8/pyjava.egg-info/SOURCES.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2023-09-19 00:09:48.000000 pyjava-0.6.8/pyjava.egg-info/dependency_links.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        7 2023-09-19 00:09:48.000000 pyjava-0.6.8/pyjava.egg-info/top_level.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       79 2023-09-19 00:09:48.306370 pyjava-0.6.8/setup.cfg
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2955 2023-04-11 04:53:45.000000 pyjava-0.6.8/setup.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-25 08:44:50.237890 pyjava-0.6.9/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      597 2023-09-25 08:44:50.237890 pyjava-0.6.9/PKG-INFO
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      448 2023-04-11 04:53:45.000000 pyjava-0.6.9/README.md
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-25 08:44:50.233890 pyjava-0.6.9/pyjava/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2612 2023-04-11 04:53:45.000000 pyjava-0.6.9/pyjava/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-25 08:44:50.233890 pyjava-0.6.9/pyjava/api/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      688 2023-04-11 04:53:45.000000 pyjava-0.6.9/pyjava/api/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16645 2023-09-18 05:38:30.000000 pyjava-0.6.9/pyjava/api/mlsql.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4524 2023-04-11 04:53:45.000000 pyjava-0.6.9/pyjava/api/serve.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-25 08:44:50.233890 pyjava-0.6.9/pyjava/cache/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.9/pyjava/cache/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      489 2023-04-11 04:53:45.000000 pyjava-0.6.9/pyjava/cache/code_cache.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42222 2023-04-11 04:53:45.000000 pyjava-0.6.9/pyjava/cloudpickle.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7048 2023-04-17 05:24:46.000000 pyjava-0.6.9/pyjava/daemon.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-25 08:44:50.233890 pyjava-0.6.9/pyjava/data/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.9/pyjava/data/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1185 2023-04-11 04:53:45.000000 pyjava-0.6.9/pyjava/data/datasource.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-25 08:44:50.233890 pyjava-0.6.9/pyjava/datatype/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.9/pyjava/datatype/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    64554 2023-04-11 04:53:45.000000 pyjava-0.6.9/pyjava/datatype/types.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2190 2023-04-11 04:53:45.000000 pyjava-0.6.9/pyjava/rayfix.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30195 2023-04-11 04:53:45.000000 pyjava-0.6.9/pyjava/serializers.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-25 08:44:50.237890 pyjava-0.6.9/pyjava/storage/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.9/pyjava/storage/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2825 2023-04-24 06:01:20.000000 pyjava-0.6.9/pyjava/storage/streaming_tar.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-25 08:44:50.237890 pyjava-0.6.9/pyjava/udf/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10721 2023-09-18 16:30:35.000000 pyjava-0.6.9/pyjava/udf/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1619 2023-09-25 08:37:30.000000 pyjava-0.6.9/pyjava/udf/store.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3990 2023-06-23 13:03:45.000000 pyjava-0.6.9/pyjava/utils.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      828 2023-09-25 08:44:31.000000 pyjava-0.6.9/pyjava/version.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6457 2023-04-18 03:10:44.000000 pyjava-0.6.9/pyjava/worker.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-09-25 08:44:50.233890 pyjava-0.6.9/pyjava.egg-info/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      597 2023-09-25 08:44:50.000000 pyjava-0.6.9/pyjava.egg-info/PKG-INFO
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      616 2023-09-25 08:44:50.000000 pyjava-0.6.9/pyjava.egg-info/SOURCES.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2023-09-25 08:44:50.000000 pyjava-0.6.9/pyjava.egg-info/dependency_links.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        7 2023-09-25 08:44:50.000000 pyjava-0.6.9/pyjava.egg-info/top_level.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       79 2023-09-25 08:44:50.237890 pyjava-0.6.9/setup.cfg
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2955 2023-04-11 04:53:45.000000 pyjava-0.6.9/setup.py
```

### Comparing `pyjava-0.6.8/PKG-INFO` & `pyjava-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjava
-Version: 0.6.8
+Version: 0.6.9
 Summary: PyJava Python API
 Home-page: https://github.com/allwefantasy/pyjava
 Author: allwefantasy
 Author-email: allwefantasy@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyjava-0.6.8/pyjava/__init__.py` & `pyjava-0.6.9/pyjava/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.8/pyjava/api/__init__.py` & `pyjava-0.6.9/pyjava/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.8/pyjava/api/mlsql.py` & `pyjava-0.6.9/pyjava/api/mlsql.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.8/pyjava/api/serve.py` & `pyjava-0.6.9/pyjava/api/serve.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.8/pyjava/cloudpickle.py` & `pyjava-0.6.9/pyjava/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.8/pyjava/daemon.py` & `pyjava-0.6.9/pyjava/daemon.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.8/pyjava/data/datasource.py` & `pyjava-0.6.9/pyjava/data/datasource.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.8/pyjava/datatype/types.py` & `pyjava-0.6.9/pyjava/datatype/types.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.8/pyjava/rayfix.py` & `pyjava-0.6.9/pyjava/rayfix.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.8/pyjava/serializers.py` & `pyjava-0.6.9/pyjava/serializers.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.8/pyjava/storage/streaming_tar.py` & `pyjava-0.6.9/pyjava/storage/streaming_tar.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.8/pyjava/udf/__init__.py` & `pyjava-0.6.9/pyjava/udf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.8/pyjava/udf/store.py` & `pyjava-0.6.9/pyjava/udf/store.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,8 +32,9 @@
     queue = asyncio.Queue(1000)
     worker_task = asyncio.create_task(worker(queue,udf_name,model_refs))
     producer_task = asyncio.create_task(producer(RayContext.collect_from(model_servers), udf_name,queue))    
     await asyncio.gather(producer_task,worker_task)
     print_flush(f"MODEL[{udf_name}] UDFMaster push model to object store cost {time.time() - time1} seconds") 
 
 def transfer_to_ob(udf_name, conf,model_refs):
-    asyncio.run(_transfer_to_ob(udf_name, conf,model_refs))
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(_transfer_to_ob(udf_name, conf,model_refs))
```

### Comparing `pyjava-0.6.8/pyjava/utils.py` & `pyjava-0.6.9/pyjava/utils.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.8/pyjava/version.py` & `pyjava-0.6.9/pyjava/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.6.8"
+__version__ = "0.6.9"
```

### Comparing `pyjava-0.6.8/pyjava/worker.py` & `pyjava-0.6.9/pyjava/worker.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.8/pyjava.egg-info/PKG-INFO` & `pyjava-0.6.9/pyjava.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjava
-Version: 0.6.8
+Version: 0.6.9
 Summary: PyJava Python API
 Home-page: https://github.com/allwefantasy/pyjava
 Author: allwefantasy
 Author-email: allwefantasy@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyjava-0.6.8/pyjava.egg-info/SOURCES.txt` & `pyjava-0.6.9/pyjava.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.8/setup.py` & `pyjava-0.6.9/setup.py`

 * *Files identical despite different names*

