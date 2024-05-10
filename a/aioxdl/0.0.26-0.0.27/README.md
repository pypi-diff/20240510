# Comparing `tmp/aioxdl-0.0.26.tar.gz` & `tmp/aioxdl-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.26.tar", last modified: Thu May  2 20:03:50 2024, max compression
+gzip compressed data, was "aioxdl-0.0.27.tar", last modified: Fri May 10 11:29:10 2024, max compression
```

## Comparing `aioxdl-0.0.26.tar` & `aioxdl-0.0.27.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:50.230550 aioxdl-0.0.26/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 20:03:44.000000 aioxdl-0.0.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-02 20:03:50.230550 aioxdl-0.0.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-02 20:03:44.000000 aioxdl-0.0.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:50.226550 aioxdl-0.0.26/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 20:03:44.000000 aioxdl-0.0.26/aioxdl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:50.226550 aioxdl-0.0.26/aioxdl/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 20:03:44.000000 aioxdl-0.0.26/aioxdl/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-02 20:03:44.000000 aioxdl-0.0.26/aioxdl/functions/function01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:50.230550 aioxdl-0.0.26/aioxdl/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 20:03:44.000000 aioxdl-0.0.26/aioxdl/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-02 20:03:44.000000 aioxdl-0.0.26/aioxdl/modules/module01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:50.230550 aioxdl-0.0.26/aioxdl/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 20:03:44.000000 aioxdl-0.0.26/aioxdl/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 20:03:44.000000 aioxdl-0.0.26/aioxdl/scripts/en.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:50.230550 aioxdl-0.0.26/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-02 20:03:50.000000 aioxdl-0.0.26/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 20:03:50.000000 aioxdl-0.0.26/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:03:50.000000 aioxdl-0.0.26/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 20:03:50.000000 aioxdl-0.0.26/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 20:03:50.000000 aioxdl-0.0.26/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:03:50.230550 aioxdl-0.0.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-02 20:03:44.000000 aioxdl-0.0.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:29:10.093124 aioxdl-0.0.27/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 11:29:01.000000 aioxdl-0.0.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-10 11:29:10.093124 aioxdl-0.0.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-10 11:29:01.000000 aioxdl-0.0.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:29:10.089124 aioxdl-0.0.27/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-10 11:29:01.000000 aioxdl-0.0.27/aioxdl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:29:10.089124 aioxdl-0.0.27/aioxdl/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-10 11:29:01.000000 aioxdl-0.0.27/aioxdl/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-10 11:29:01.000000 aioxdl-0.0.27/aioxdl/functions/function01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:29:10.093124 aioxdl-0.0.27/aioxdl/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-10 11:29:01.000000 aioxdl-0.0.27/aioxdl/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-10 11:29:01.000000 aioxdl-0.0.27/aioxdl/modules/module01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:29:10.093124 aioxdl-0.0.27/aioxdl/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 11:29:01.000000 aioxdl-0.0.27/aioxdl/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 11:29:01.000000 aioxdl-0.0.27/aioxdl/scripts/en.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:29:10.093124 aioxdl-0.0.27/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-10 11:29:10.000000 aioxdl-0.0.27/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 11:29:10.000000 aioxdl-0.0.27/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:29:10.000000 aioxdl-0.0.27/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 11:29:10.000000 aioxdl-0.0.27/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 11:29:10.000000 aioxdl-0.0.27/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:29:10.093124 aioxdl-0.0.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 11:29:01.000000 aioxdl-0.0.27/setup.py
```

### Comparing `aioxdl-0.0.26/LICENSE` & `aioxdl-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.26/PKG-INFO` & `aioxdl-0.0.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.26
+Version: 0.0.27
 Summary: Python fast downloader
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.26 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.27 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
```

### Comparing `aioxdl-0.0.26/README.md` & `aioxdl-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.26/aioxdl/__init__.py` & `aioxdl-0.0.27/aioxdl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "aioxdl"
-version = "0.0.26"
+version = "0.0.27"
 
 install = ["aiohttp", "yt-dlp"]
 
 contact = "clintonabrahamc@gmail.com"
 
 classis = ['Natural Language :: English',
           'Intended Audience :: Developers',
```

### Comparing `aioxdl-0.0.26/aioxdl/modules/module01.py` & `aioxdl-0.0.27/aioxdl/modules/module01.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,40 +2,43 @@
 from ..functions import Hkeys
 from ..scripts import Scripted
 from yt_dlp import YoutubeDL, DownloadError
 #=========================================================================================================
 
 class Aioxdl:
 
-    def __init__(self, **kwargs):
+    def __init__(self, chunk=1024, timeout=1000, message=None):
         self.dsizes = 0
         self.tsizes = 0
+        self.errors = None
+        self.chunks = chunk
+        self.otimes = timeout
+        self.mesage = message
         self.stimes = time.time()
         self.comand = Hkeys.DATA01
         self.fnames = Hkeys.DATA02
-        self.chunks = kwargs.get("chunk", 1024)
-        self.errors = kwargs.get("errors", None)
-        self.mesage = kwargs.get("message", None)
-        self.otimes = kwargs.get("timeout", 1000)
 
 #=========================================================================================================
 
-    async def download(self, url, location, timeout, progress):
+    async def download(self, url, location, progress):
         async with aiohttp.ClientSession() as session:
-            async with session.get(url, timeout=timeout) as response:
+            async with session.get(url, timeout=self.otimes) as response:
                 self.tsizes += await self.getsizes(response)
                 with open(location, "wb") as handlexo:
                     while True:
                         chunks = await response.content.read(self.chunks)
                         if not chunks:
                             break
                         handlexo.write(chunks)
                         self.dsizes += self.chunks
                         try: await self.display(progress)
                         except ZeroDivisionError: pass
+                        except Exception as errors:
+                            self.errors = errors
+                            break
 
                 await response.release()
                 return location if location else None
 
 #=========================================================================================================
 
     async def filename(self, filelink):
@@ -64,15 +67,15 @@
             await progress(self.stimes, self.tsizes, self.dsizes)
         else: pass
 
 #=========================================================================================================
 
     async def start(self, url, location, progress=None):
         try:
-            location = await self.download(url, location, self.otimes, progress)
+            location = await self.download(url, location, progress)
         except aiohttp.ClientConnectorError as errors:
             self.errors = errors
         except asyncio.TimeoutError:
             self.errors = Scripted.DATA01
         except Exception as errors:
             self.errors = errors
```

### Comparing `aioxdl-0.0.26/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.27/aioxdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.26
+Version: 0.0.27
 Summary: Python fast downloader
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.26 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.27 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
```

### Comparing `aioxdl-0.0.26/setup.py` & `aioxdl-0.0.27/setup.py`

 * *Files identical despite different names*

