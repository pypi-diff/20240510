# Comparing `tmp/celery_streaming_result-0.1.1.tar.gz` & `tmp/celery_streaming_result-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery_streaming_result-0.1.1.tar", last modified: Mon Apr 15 14:28:23 2024, max compression
+gzip compressed data, was "celery_streaming_result-0.1.2.tar", last modified: Fri May 10 15:49:47 2024, max compression
```

## Comparing `celery_streaming_result-0.1.1.tar` & `celery_streaming_result-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-15 14:28:23.240257 celery_streaming_result-0.1.1/
--rw-r--r--   0 test       (501) staff       (20)     1036 2024-04-13 13:33:44.000000 celery_streaming_result-0.1.1/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      167 2024-04-13 13:35:03.000000 celery_streaming_result-0.1.1/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     3060 2024-04-15 14:28:23.240128 celery_streaming_result-0.1.1/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     2410 2024-04-15 14:16:34.000000 celery_streaming_result-0.1.1/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-15 14:28:23.238978 celery_streaming_result-0.1.1/celery_streaming_result/
--rw-r--r--   0 test       (501) staff       (20)       20 2024-04-13 12:33:22.000000 celery_streaming_result-0.1.1/celery_streaming_result/__init__.py
--rw-r--r--   0 test       (501) staff       (20)     7022 2024-04-15 14:17:11.000000 celery_streaming_result-0.1.1/celery_streaming_result/core.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-15 14:28:23.239902 celery_streaming_result-0.1.1/celery_streaming_result.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     3060 2024-04-15 14:28:23.000000 celery_streaming_result-0.1.1/celery_streaming_result.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      403 2024-04-15 14:28:23.000000 celery_streaming_result-0.1.1/celery_streaming_result.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-04-15 14:28:23.000000 celery_streaming_result-0.1.1/celery_streaming_result.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-04-15 14:28:23.000000 celery_streaming_result-0.1.1/celery_streaming_result.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       29 2024-04-15 14:28:23.000000 celery_streaming_result-0.1.1/celery_streaming_result.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       24 2024-04-15 14:28:23.000000 celery_streaming_result-0.1.1/celery_streaming_result.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)       29 2024-04-15 13:57:28.000000 celery_streaming_result-0.1.1/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2024-04-15 14:28:23.240302 celery_streaming_result-0.1.1/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1473 2024-04-15 01:21:50.000000 celery_streaming_result-0.1.1/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-10 15:49:47.665631 celery_streaming_result-0.1.2/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-04-13 13:33:44.000000 celery_streaming_result-0.1.2/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      167 2024-04-13 13:35:03.000000 celery_streaming_result-0.1.2/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     3059 2024-05-10 15:49:47.665511 celery_streaming_result-0.1.2/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     2448 2024-05-09 09:54:12.000000 celery_streaming_result-0.1.2/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-10 15:49:47.664503 celery_streaming_result-0.1.2/celery_streaming_result/
+-rw-r--r--   0 test       (501) staff       (20)       20 2024-04-13 12:33:22.000000 celery_streaming_result-0.1.2/celery_streaming_result/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)     8675 2024-05-09 09:54:06.000000 celery_streaming_result-0.1.2/celery_streaming_result/core.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-10 15:49:47.665330 celery_streaming_result-0.1.2/celery_streaming_result.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     3059 2024-05-10 15:49:47.000000 celery_streaming_result-0.1.2/celery_streaming_result.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      403 2024-05-10 15:49:47.000000 celery_streaming_result-0.1.2/celery_streaming_result.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-10 15:49:47.000000 celery_streaming_result-0.1.2/celery_streaming_result.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-10 15:49:47.000000 celery_streaming_result-0.1.2/celery_streaming_result.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       29 2024-05-10 15:49:47.000000 celery_streaming_result-0.1.2/celery_streaming_result.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       24 2024-05-10 15:49:47.000000 celery_streaming_result-0.1.2/celery_streaming_result.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)       29 2024-04-15 13:57:28.000000 celery_streaming_result-0.1.2/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-10 15:49:47.665669 celery_streaming_result-0.1.2/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1473 2024-05-08 07:38:12.000000 celery_streaming_result-0.1.2/setup.py
```

### Comparing `celery_streaming_result-0.1.1/LICENSE` & `celery_streaming_result-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `celery_streaming_result-0.1.1/PKG-INFO` & `celery_streaming_result-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: celery_streaming_result
-Version: 0.1.1
+Version: 0.1.2
 Summary: Celery任务结果分片管理
-Home-page: UNKNOWN
 Author: Zhou WeiKe
 Maintainer: Zhou WeiKe
 License: MIT
 Keywords: celery_streaming_result,celery,streaming result
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -117,8 +115,10 @@
 1. 首次发布。
 
 ### v0.1.1
 
 1. 添加asyncio支持。
 1. 获取结果支持on_finished回调。
 
+### v0.1.2
 
+1. 流式中断支持。
```

### Comparing `celery_streaming_result-0.1.1/README.md` & `celery_streaming_result-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -97,7 +97,11 @@
 
 1. 首次发布。
 
 ### v0.1.1
 
 1. 添加asyncio支持。
 1. 获取结果支持on_finished回调。
+
+### v0.1.2
+
+1. 流式中断支持。
```

### Comparing `celery_streaming_result-0.1.1/celery_streaming_result/core.py` & `celery_streaming_result-0.1.2/celery_streaming_result/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     "ReadCeleryStreamingResultTimeout",
     "CeleryStreamingResultManager",
     "start_celery_task_async",
     "get_celery_task_result_async",
 ]
 
 DEFAULT_ENDED_CHUNK = "this:is:the:celery:streaming:result:ended:chunk:b53127b4-ba43-4ff4-aba4-2134b17b9006"
+DEFAULT_BREAK_CHUNK = "this:is:the:celery:streaming:result:break:chunk:ad17e201-59a9-405d-be8e-9be91caa6875"
 
 
 class ReadCeleryStreamingResultTimeout(RuntimeError):
     args = (124, "读取分片结果超时")
 
 
 class CeleryStreamingResultManager(object):
@@ -48,14 +49,15 @@
     """
 
     def __init__(
         self,
         store,
         result_key_template=None,
         ended_chunk=None,
+        break_chunk=None,
         encode=None,
         decode=None,
         expires=60 * 60 * 24,
     ):
         """基于Redis的Celery任务结果分片管理器。
 
         @parameter: store Redis实例。
@@ -72,48 +74,74 @@
             设置一个超时时间，避免有效数据在redis积累造成内存泄漏。
         """
         self.store = store
         self.result_key_template = (
             result_key_template or "celery-streaming-results:{task_id}"
         )
         self.ended_chunk = ended_chunk or DEFAULT_ENDED_CHUNK
+        self.break_chunk = break_chunk or DEFAULT_BREAK_CHUNK
         if encode is None:
             self.encode = msgpack.dumps
         else:
             self.encode = encode
         if decode is None:
             self.decode = msgpack.loads
         else:
             self.decode = decode
         self.expires = expires
 
+    def get_task_id(self, task):
+        if hasattr(task, "request"):
+            return task.request.id
+        if hasattr(task, "task_id"):
+            return task.task_id
+        raise RuntimeError("无效的task实例...")
+
     def append_result_chunk(self, task, chunk):
         """输出分片结果。"""
-        result_key = self.result_key_template.format(task_id=task.request.id)
+        task_id = self.get_task_id(task)
+        result_key = self.result_key_template.format(task_id=task_id)
         self.store.lpush(result_key, self.encode(chunk))
         self.store.expire(result_key, self.expires)
 
     async def async_append_result_chunk(self, task, chunk):
         """输出分片结果。"""
-        result_key = self.result_key_template.format(task_id=task.request.id)
+        task_id = self.get_task_id(task)
+        result_key = self.result_key_template.format(task_id=task_id)
         await self.store.lpush(result_key, self.encode(chunk))
         await self.store.expire(result_key, self.expires)
 
     def append_ended_chunk(self, task):
         """输出分片结果结束标识。"""
-        result_key = self.result_key_template.format(task_id=task.request.id)
+        task_id = self.get_task_id(task)
+        result_key = self.result_key_template.format(task_id=task_id)
         self.store.lpush(result_key, self.encode(self.ended_chunk))
         self.store.expire(result_key, self.expires)
 
     async def async_append_ended_chunk(self, task):
         """输出分片结果结束标识。"""
-        result_key = self.result_key_template.format(task_id=task.request.id)
+        task_id = self.get_task_id(task)
+        result_key = self.result_key_template.format(task_id=task_id)
         await self.store.lpush(result_key, self.encode(self.ended_chunk))
         await self.store.expire(result_key, self.expires)
 
+    def append_break_chunk(self, task):
+        """输出中断标识。"""
+        task_id = self.get_task_id(task)
+        result_key = self.result_key_template.format(task_id=task_id)
+        self.store.lpush(result_key, self.encode(self.break_chunk))
+        self.store.expire(result_key, self.expires)
+
+    async def async_append_break_chunk(self, task):
+        """输出中断标识。"""
+        task_id = self.get_task_id(task)
+        result_key = self.result_key_template.format(task_id=task_id)
+        await self.store.lpush(result_key, self.encode(self.break_chunk))
+        await self.store.expire(result_key, self.expires)
+
     def get_result_chunks(
         self,
         celery_async_task,
         total_timeout=0,
         read_timeout=0,
         interval=1,
         on_finished=None,
@@ -140,20 +168,25 @@
                     if (read_timeout != 0) and (time.time() - rtime > read_timeout):
                         raise ReadCeleryStreamingResultTimeout()
             else:
                 rtime = None
             if result is None:
                 continue
             result = self.decode(result[1])
-            if result != self.ended_chunk:
-                yield result
-            else:
+            if result == self.break_chunk:
+                if on_finished:
+                    on_finished(celery_async_task, break_flag=True)
+                yield self.break_chunk
+                return
+            elif result == self.ended_chunk:
                 if on_finished:
-                    on_finished(celery_async_task)
+                    on_finished(celery_async_task, break_flag=False)
                 return
+            else:
+                yield result
 
     async def async_get_result_chunks(
         self,
         celery_async_task,
         total_timeout=0,
         read_timeout=0,
         interval=1,
@@ -173,20 +206,25 @@
                     if (read_timeout != 0) and (time.time() - rtime > read_timeout):
                         raise ReadCeleryStreamingResultTimeout()
             else:
                 rtime = None
             if result is None:
                 continue
             result = self.decode(result[1])
-            if result != self.ended_chunk:
-                yield result
-            else:
+            if result == self.break_chunk:
                 if on_finished:
-                    await on_finished(celery_async_task)
+                    await on_finished(celery_async_task, break_flag=True)
+                yield self.break_chunk
                 return
+            elif result == self.ended_chunk:
+                if on_finished:
+                    await on_finished(celery_async_task, break_flag=False)
+                return
+            else:
+                yield result
 
 
 async def start_celery_task_async(celery_task, *args, **kwargs):
     """使用异步方法启动一个Celery任务。"""
     result = await sync_to_async(celery_task.delay)(*args, **kwargs)
     return result
```

### Comparing `celery_streaming_result-0.1.1/celery_streaming_result.egg-info/PKG-INFO` & `celery_streaming_result-0.1.2/celery_streaming_result.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: celery-streaming-result
-Version: 0.1.1
+Version: 0.1.2
 Summary: Celery任务结果分片管理
-Home-page: UNKNOWN
 Author: Zhou WeiKe
 Maintainer: Zhou WeiKe
 License: MIT
 Keywords: celery_streaming_result,celery,streaming result
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -117,8 +115,10 @@
 1. 首次发布。
 
 ### v0.1.1
 
 1. 添加asyncio支持。
 1. 获取结果支持on_finished回调。
 
+### v0.1.2
 
+1. 流式中断支持。
```

### Comparing `celery_streaming_result-0.1.1/setup.py` & `celery_streaming_result-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 requires = []
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires += [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="celery_streaming_result",
-    version="0.1.1",
+    version="0.1.2",
     description="Celery任务结果分片管理",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Zhou WeiKe",
     maintainer="Zhou WeiKe",
     license="MIT",
     license_files=("LICENSE",),
```

