# Comparing `tmp/indralib-0.0.6.tar.gz` & `tmp/indralib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indralib-0.0.6.tar", last modified: Thu May  9 15:58:59 2024, max compression
+gzip compressed data, was "indralib-0.0.7.tar", last modified: Thu May  9 16:28:29 2024, max compression
```

## Comparing `indralib-0.0.6.tar` & `indralib-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 15:58:59.339834 indralib-0.0.6/
--rw-r--r--   0 dsc        (501) staff       (20)      627 2024-05-09 15:58:59.339657 indralib-0.0.6/PKG-INFO
--rw-r--r--   0 dsc        (501) staff       (20)       52 2024-05-09 14:18:10.000000 indralib-0.0.6/README.md
--rw-r--r--   0 dsc        (501) staff       (20)      676 2024-05-09 15:57:52.000000 indralib-0.0.6/pyproject.toml
--rw-r--r--   0 dsc        (501) staff       (20)       38 2024-05-09 15:58:59.339874 indralib-0.0.6/setup.cfg
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 15:58:59.337731 indralib-0.0.6/src/
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 15:58:59.338678 indralib-0.0.6/src/indralib/
--rw-r--r--   0 dsc        (501) staff       (20)        0 2024-05-09 14:14:09.000000 indralib-0.0.6/src/indralib/__init__.py
--rw-r--r--   0 dsc        (501) staff       (20)    23177 2024-05-09 14:46:29.000000 indralib-0.0.6/src/indralib/indra_client.py
--rw-r--r--   0 dsc        (501) staff       (20)    17753 2024-05-09 14:46:36.000000 indralib-0.0.6/src/indralib/indra_downloader.py
--rw-r--r--   0 dsc        (501) staff       (20)     3214 2024-05-09 15:30:32.000000 indralib-0.0.6/src/indralib/indra_event.py
--rw-r--r--   0 dsc        (501) staff       (20)     2720 2024-05-09 14:46:45.000000 indralib-0.0.6/src/indralib/indra_module.py
--rw-r--r--   0 dsc        (501) staff       (20)    13670 2024-05-09 14:46:52.000000 indralib-0.0.6/src/indralib/indra_time.py
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 15:58:59.339465 indralib-0.0.6/src/indralib.egg-info/
--rw-r--r--   0 dsc        (501) staff       (20)      627 2024-05-09 15:58:59.000000 indralib-0.0.6/src/indralib.egg-info/PKG-INFO
--rw-r--r--   0 dsc        (501) staff       (20)      374 2024-05-09 15:58:59.000000 indralib-0.0.6/src/indralib.egg-info/SOURCES.txt
--rw-r--r--   0 dsc        (501) staff       (20)        1 2024-05-09 15:58:59.000000 indralib-0.0.6/src/indralib.egg-info/dependency_links.txt
--rw-r--r--   0 dsc        (501) staff       (20)       17 2024-05-09 15:58:59.000000 indralib-0.0.6/src/indralib.egg-info/requires.txt
--rw-r--r--   0 dsc        (501) staff       (20)        9 2024-05-09 15:58:59.000000 indralib-0.0.6/src/indralib.egg-info/top_level.txt
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 16:28:29.282010 indralib-0.0.7/
+-rw-r--r--   0 dsc        (501) staff       (20)      627 2024-05-09 16:28:29.281823 indralib-0.0.7/PKG-INFO
+-rw-r--r--   0 dsc        (501) staff       (20)       52 2024-05-09 14:18:10.000000 indralib-0.0.7/README.md
+-rw-r--r--   0 dsc        (501) staff       (20)      676 2024-05-09 16:27:50.000000 indralib-0.0.7/pyproject.toml
+-rw-r--r--   0 dsc        (501) staff       (20)       38 2024-05-09 16:28:29.282054 indralib-0.0.7/setup.cfg
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 16:28:29.279888 indralib-0.0.7/src/
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 16:28:29.280827 indralib-0.0.7/src/indralib/
+-rw-r--r--   0 dsc        (501) staff       (20)        0 2024-05-09 14:14:09.000000 indralib-0.0.7/src/indralib/__init__.py
+-rw-r--r--   0 dsc        (501) staff       (20)    23527 2024-05-09 16:27:31.000000 indralib-0.0.7/src/indralib/indra_client.py
+-rw-r--r--   0 dsc        (501) staff       (20)    17753 2024-05-09 14:46:36.000000 indralib-0.0.7/src/indralib/indra_downloader.py
+-rw-r--r--   0 dsc        (501) staff       (20)     3214 2024-05-09 15:30:32.000000 indralib-0.0.7/src/indralib/indra_event.py
+-rw-r--r--   0 dsc        (501) staff       (20)     2720 2024-05-09 14:46:45.000000 indralib-0.0.7/src/indralib/indra_module.py
+-rw-r--r--   0 dsc        (501) staff       (20)    13670 2024-05-09 14:46:52.000000 indralib-0.0.7/src/indralib/indra_time.py
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 16:28:29.281634 indralib-0.0.7/src/indralib.egg-info/
+-rw-r--r--   0 dsc        (501) staff       (20)      627 2024-05-09 16:28:29.000000 indralib-0.0.7/src/indralib.egg-info/PKG-INFO
+-rw-r--r--   0 dsc        (501) staff       (20)      374 2024-05-09 16:28:29.000000 indralib-0.0.7/src/indralib.egg-info/SOURCES.txt
+-rw-r--r--   0 dsc        (501) staff       (20)        1 2024-05-09 16:28:29.000000 indralib-0.0.7/src/indralib.egg-info/dependency_links.txt
+-rw-r--r--   0 dsc        (501) staff       (20)       17 2024-05-09 16:28:29.000000 indralib-0.0.7/src/indralib.egg-info/requires.txt
+-rw-r--r--   0 dsc        (501) staff       (20)        9 2024-05-09 16:28:29.000000 indralib-0.0.7/src/indralib.egg-info/top_level.txt
```

### Comparing `indralib-0.0.6/pyproject.toml` & `indralib-0.0.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "indralib"
-version = "0.0.6"
+version = "0.0.7"
 authors = [{ name = "Dominik Schlösser", email = "dominik.schloesser@gmail.com" }]
 description = "Client for the Indrajala system"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `indralib-0.0.6/src/indralib/indra_client.py` & `indralib-0.0.7/src/indralib/indra_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
             self.module_name = module_name
         self.websocket = None
         self.verbose = verbose
         self.trx = {}
         self.recv_queue = asyncio.Queue()
         self.recv_task = None
         self.initialized = False
+        self.error_shown = False
         if profile is not None and profile.lower() in ["default", "none"]:
             profile = None
         if config_file is not None and config_file != "":
             self.initialized = self.get_config(config_file, verbose=self.verbose)
         elif uri is not None and uri != "":
             self.initialized = True
             self.uri = uri
@@ -205,14 +206,15 @@
             self.log.error(f"Could not connect to {self.uri}: {e}")
             self.websocket = None
             return None
         self.recv_queue.empty()
         self.recv_task = asyncio.create_task(self.fn_recv_task())
         self.session_id = None
         self.username = None
+        self.error_shown = False
         return self.websocket
 
     async def fn_recv_task(self):
         """Receive task"""
         while True:
             try:
                 message = await self.websocket.recv()
@@ -244,15 +246,19 @@
                 await self.recv_queue.put(ie)
         self.recv_task = None
         return
 
     async def send_event(self, event):
         """Send event"""
         if self.initialized is False:
-            self.log.error("Indrajala send_event(): connection data not initialized!")
+            if self.error_shown is False:
+                self.error_shown = True
+                self.log.error(
+                    "Indrajala send_event(): connection data not initialized!"
+                )
             return False
         if self.websocket is None:
             self.log.error(
                 "Websocket not initialized, please call init_connection() first!"
             )
             return False
         if isinstance(event, IndraEvent) is False:
@@ -264,15 +270,19 @@
                 "future": replyEventFuture,
                 "start_time": time.time(),
             }
             self.trx[event.uuid4] = fRec
             self.log.debug("Future: ", replyEventFuture)
         else:
             replyEventFuture = None
-        await self.websocket.send(event.to_json())
+        try:
+            await self.websocket.send(event.to_json())
+        except Exception as e:
+            self.log.error(f"Could not send message: {e}, uninitialized.")
+            self.initialized = False
         return replyEventFuture
 
     async def recv_event(self, timeout=None):
         """Receive event"""
         if self.initialized is False:
             self.log.error("Indrajala recv_event(): connection data not initialized!")
             return None
```

### Comparing `indralib-0.0.6/src/indralib/indra_downloader.py` & `indralib-0.0.7/src/indralib/indra_downloader.py`

 * *Files identical despite different names*

### Comparing `indralib-0.0.6/src/indralib/indra_event.py` & `indralib-0.0.7/src/indralib/indra_event.py`

 * *Files identical despite different names*

### Comparing `indralib-0.0.6/src/indralib/indra_module.py` & `indralib-0.0.7/src/indralib/indra_module.py`

 * *Files identical despite different names*

### Comparing `indralib-0.0.6/src/indralib/indra_time.py` & `indralib-0.0.7/src/indralib/indra_time.py`

 * *Files identical despite different names*

