# Comparing `tmp/openagents_node_sdk-0.1.5.tar.gz` & `tmp/openagents_node_sdk-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openagents_node_sdk-0.1.5.tar", last modified: Mon May  6 15:52:11 2024, max compression
+gzip compressed data, was "openagents_node_sdk-0.2.tar", last modified: Fri May 10 07:00:01 2024, max compression
```

## Comparing `openagents_node_sdk-0.1.5.tar` & `openagents_node_sdk-0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:52:11.541254 openagents_node_sdk-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-06 15:52:11.541254 openagents_node_sdk-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:52:11.541254 openagents_node_sdk-0.1.5/openagents/
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/Disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/DiskReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/DiskWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8845 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/JobRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/NodeConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/OpenAgentsNode.py
--rw-r--r--   0 runner    (1001) docker     (127)    16537 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/RunnerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:52:11.541254 openagents_node_sdk-0.1.5/openagents_node_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-06 15:52:11.000000 openagents_node_sdk-0.1.5/openagents_node_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-06 15:52:11.000000 openagents_node_sdk-0.1.5/openagents_node_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:52:11.000000 openagents_node_sdk-0.1.5/openagents_node_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-06 15:52:11.000000 openagents_node_sdk-0.1.5/openagents_node_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 15:52:11.000000 openagents_node_sdk-0.1.5/openagents_node_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:52:11.541254 openagents_node_sdk-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:00:01.548777 openagents_node_sdk-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-10 07:00:01.548777 openagents_node_sdk-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:00:01.548777 openagents_node_sdk-0.2/openagents/
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/Disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/DiskReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/DiskWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/JobContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/JobRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/NodeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/OpenAgentsNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/RunnerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:00:01.548777 openagents_node_sdk-0.2/openagents_node_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-10 07:00:01.000000 openagents_node_sdk-0.2/openagents_node_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-10 07:00:01.000000 openagents_node_sdk-0.2/openagents_node_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:00:01.000000 openagents_node_sdk-0.2/openagents_node_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 07:00:01.000000 openagents_node_sdk-0.2/openagents_node_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 07:00:01.000000 openagents_node_sdk-0.2/openagents_node_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 07:00:01.548777 openagents_node_sdk-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/setup.py
```

### Comparing `openagents_node_sdk-0.1.5/LICENSE` & `openagents_node_sdk-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.5/README.md` & `openagents_node_sdk-0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -13,40 +13,33 @@
 
 ```python
 from openagents import JobRunner,OpenAgentsNode,NodeConfig,RunnerConfig
 
 # Define a runner
 class MyRunner (JobRunner):
     def __init__(self):
-        # Set the runner metadata, template and filters
+        # Set the runner metadata, template and filter
         super().__init__(\
             RunnerConfig(
                 meta={
                     "kind":5003,
                     "name":"My Action",
                     "description":"This is a new action"
                     "tos": "https://example.com/tos",
                     "privacy": "https://example.com/privacy",
                     "picture": "https://example.com/icon.png",
                     "tags": ["tag1","tag2"]
                     "website": "https://example.com",
                     "author": "John Doe",
                 },
-                filters=[ 
-                    {
-                        "filterByKind":5003,
-                        #AND
-                        "filterByRunOn": "my-new-action"
-                    }, # OR
-                    {
-                        "filterByKind": 5003,
-                        #AND
-                        "filterByRunOn": "my-new-action-alt"
-                    }
-                ],
+                filter={
+                    "filterByKind":5003,
+                    #AND
+                    "filterByRunOn": "my-new-action"
+                },
                 template="""
                 {
                     "kind": {{meta.kind}},
                     "created_at": {{sys.timestamp_seconds}},
                     "tags": [
                         ["param","run-on", "my-new-action" ],                             
                         ["param", "k", "{{in.k}}"],
@@ -57,34 +50,34 @@
                         ["expiration", "{{sys.expiration_timestamp_seconds}}"],
                     ],
                     "content":""
                 }""",
                 sockets={
                     "in": {
                         "k": {
-                            "type":"number",
+                            "title": "K",
                             "description":"This is a number"
-                            "default": "0"
+                            "type":"integer",
+                            "default": 0,
                         },
                         "queries": {
+                            "title": "Queries",
                             "type":"array",
                             "description":"This is an array of queries",
-                            "schema": {
-                                "value":{
-                                    "type":"string",
-                                    "description":"This is a query value"
-                                }# Last item in schema is repeated for any remaining items
+                            "items": {
+                                "type":"string"
                             }
                         }
                     },
                     "out": {
-                        "content": {
+                        "contentType": {
+                            "title": "Content Type",
                             "type": "string",
                             "description": "The content of the event",
-                            "value": "application/json"
+                            "default": "application/json"
                         }
                     }
                 }
             )
         )
```

### Comparing `openagents_node_sdk-0.1.5/openagents/Disk.py` & `openagents_node_sdk-0.2/openagents/Disk.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.5/openagents/DiskReader.py` & `openagents_node_sdk-0.2/openagents/DiskReader.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.5/openagents/DiskWriter.py` & `openagents_node_sdk-0.2/openagents/DiskWriter.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.5/openagents/JobRunner.py` & `openagents_node_sdk-0.2/openagents/JobContext.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,62 @@
 
-from .Logger import Logger
-from .Disk import Disk
 from openagents_grpc_proto import rpc_pb2_grpc
 from openagents_grpc_proto import rpc_pb2
+from .Logger import Logger
+from .Disk import Disk
 from .RunnerConfig import RunnerConfig
 import time
 import os
 import json
 import pickle
 from typing import Union
-class JobRunner:
-    """
-    An abstract class that represents a job runner.
-    Implementations of this class should be able to run jobs.
-    The internal logic of the runner uses these additional environment variables for configuration:
-    - CACHE_PATH: The path to store cached data. Defaults to "./cache".
-
-
 
+class JobContext:
     """
-
-    def __init__(self, metaOrConfig: Union[dict, RunnerConfig], filters:dict=None, template:dict=None, sockets:dict=None):
-        meta=None
-        if isinstance(metaOrConfig, RunnerConfig):
-            meta = metaOrConfig.getMeta()
-            filters = metaOrConfig.getFilters()
-            template = metaOrConfig.getTemplate()
-            sockets = metaOrConfig.getSockets()
-        else:
-            meta = metaOrConfig
-        self._filters = None
-        self._node = None
-        self._job = None
-        self._disksByUrl = {}
-        self._disksById = {}
-        self._diskByName = {}
-        self._template = None
-        self._meta = None
-        self._sockets = None
-        self._nextAnnouncementTimestamp = 0
-        self._cachePath = None
-
-        self.logger = Logger("JobRunner", "0", self, False)
-        self._filters = filters
-        self._meta = json.dumps(meta)
-        self._template = template
-        self._sockets = json.dumps(sockets)
+    A class that represents the context of a job.
+    """
+    def __init__(self, node: 'OpenAgentsNode',runner:'JobRunner', job: rpc_pb2.Job__pb2):
+        self.job=job
+        self._node=node
+        self.runner=runner
         
         self._cachePath = os.getenv('CACHE_PATH',  "cache")
         if not os.path.exists(self._cachePath):
             os.makedirs(self._cachePath)
 
-    
-    def getLogger(self) -> Logger:
+        self.logger=Logger(
+            self._node.getMeta()["name"]+"."+self.runner.getMeta()["name"],
+            self._node.getMeta()["version"],
+            self.job.id,
+            lambda x: self._node._log(x, self.job.id),
+        )
+
+        self._disksByUrl = {}
+        self._disksById = {}
+        self._diskByName = {}
+
+    def getLogger(self):
         """
-        Get the active logger for the runner.
-        Returns:
-            Logger: The logger for the runner.
+        Get the logger of the job.
         """
         return self.logger
 
+ 
+    def getNode(self):
+        """
+        Get the node running this job
+        """
+        return self._node
+
+    def getJob(self):
+        """
+        Get the job object.
+        """
+        return self.job
+
     
     async def cacheSet(self, key:str, value, version:int=0, expireAt:int=0, local=True, CHUNK_SIZE=1024*1024*15):
         """
         Set a value in the cache.
         Args:
             key (str): The key of the value to set.
             value (object): The value to set.
@@ -91,15 +84,15 @@
                             expireAt=expireAt,
                             version=version
                         )
                         yield request                              
                 res=await client.cacheSet(write_data())
                 return res.success
         except Exception as e:
-            self.getLogger().error("Error setting cache "+str(e))
+            self._node.getLogger().error("Error setting cache "+str(e))
             return False
         
 
     async def cacheGet(self, key:str, lastVersion = 0, local=True) -> any:
         """
         Get a value from the cache.
         Args:
@@ -128,35 +121,19 @@
                 stream = client.cacheGet(rpc_pb2.RpcCacheGetRequest(key=key, lastVersion = lastVersion))
                 async for chunk in stream:
                     if not chunk.exists:
                         return None
                     bytesOut.extend(chunk.data)
                 return pickle.loads(bytesOut)
         except Exception as e:
-            self.getLogger().error("Error getting cache "+str(e))
+            self._node.getLogger().error("Error getting cache "+str(e))
             return None
 
-    def _setNode(self, node):
-        self._node = node
-
-    def _setJob(self, job):
-        self._job = job
-
-    def _log(self, message:str):
-        """
-        Log a message to the network.
-        Shouldn't be used directly. Use getLogger().info() instead.
-        Args:
-            message (str): The message to log.
-        """
-        if self._job: message+=" for job "+self._job.id
-        if self._node: 
-            self._node._log(message, self._job.id if self._job else None)
-        
 
+    
     async def openStorage(self, url:str)->Disk:
         """
         Open a storage disk.
         Args:
             url (str): The URL of the disk.
         Returns:
             Disk: The disk object.
@@ -190,51 +167,59 @@
             encryptionKey=encryptionKey,
             includeEncryptionKeyInUrl=includeEncryptionKeyInUrl
         ))).url
         diskId =( await client.openDisk(rpc_pb2.RpcOpenDiskRequest(url=url))).diskId
         disk = Disk(id=diskId, url=url, node=self._node)
         self._disksByUrl[url] = disk
         self._disksById[diskId] = disk
-        self._diskByName[name] = disk
+        if name:self._diskByName[name] = disk
         return disk
 
-    async def postRun(self, job:rpc_pb2.Job__pb2.Job) -> None:
+    async def close(self):
         """
-        Called after the runner has finished running.
+        Close the job context.
+        Free up resources, submit pending logs.
         """
         for disk in self._disksById.values():
             await disk.close()
         for disk in self._disksByUrl.values():
             await disk.close()
         for disk in self._diskByName.values():
             await disk.close()
         self._disksById = {}
         self._disksByUrl = {}
         self._diskByName = {}
+        self.logger.close()
 
-    async def canRun(self,job:rpc_pb2.Job__pb2.Job) -> bool:
-        """
-        Check if the runner can run a job.
-        Args:
-            job (Job): The job to check.
-        Returns:
-            bool: True if the runner can run the job, False otherwise.
-        """
-        return True
-        
-    async def preRun(self, job:rpc_pb2.Job__pb2.Job)-> None:
-        """
-        Called before the runner starts running.
-        """
-        pass
 
-    async def loop(self)-> None:
-        """
-        The main loop of the runner.
-        """
-        pass
+    def getJobParamValues(self,key,default:list[str]=None)->list[str]:
+        job=self.getJob()
+        for p in job.param:
+            if p.key == key:
+                return p.value
+        return default
 
-    async def run(self, job:rpc_pb2.Job__pb2.Job) -> None:
-        """
-        Run a job.
-        """
-        pass
+    
+    def getJobParamValue(self,key,default:str=None)->str:
+        job=self.getJob()
+        for p in job.param:
+            if p.key == key:
+                return p.value[0]
+
+    def getJobInputs(self,marker:str|None=None)->list[rpc_pb2.JobInput__pb2]:
+        job=self.getJob()
+        out=[]
+        for i in job.input:
+            if marker is None or i.marker == marker:
+                out.append(i)
+        return out
+
+    def getJobInput(self,marker:str|None=None)->rpc_pb2.JobInput__pb2:
+        job=self.getJob()
+        for i in job.input:
+            if marker is None or i.marker == marker:
+                return i
+        return None
+
+    def getOutputFormat(self):
+        job=self.getJob()
+        return job.outputFormat
```

### Comparing `openagents_node_sdk-0.1.5/openagents/Logger.py` & `openagents_node_sdk-0.2/openagents/Logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,39 +53,53 @@
             log_entry[key]=meta[key]
 
         self.buffer.put(log_entry)
         if self.buffer.qsize() >= self.batchSize:
             with self.wait:
                 self.wait.notify_all()
         
- 
+    def close(self):
+        """
+        Immediately flush all the logs to OpenObserve and shutdown the logger.
+        """
+        self.flushThread.shutdown()
+        if not self.buffer.empty():
+            batch = []
+            while not self.buffer.empty():
+                batch.append(self.buffer.get())
+            self._flushToOpenObserve(batch)
+            
+        
+    def _flushToOpenObserve(self, batch):
+        try:
+            url = self.options["baseUrl"]+"/api/"+self.options["org"]+"/"+self.options["stream"]+"/_json"   
+            basicAuth = self.options["auth"]
+            if not isinstance(basicAuth, str):
+                if "username" in basicAuth and "password" in basicAuth:
+                    basicAuth = basicAuth["username"]+":"+basicAuth["password"]
+                    basicAuth = base64.b64encode(basicAuth.encode()).decode()
+            headers = {
+                'Content-Type': 'application/json',
+                "Authorization": "Basic "+basicAuth if basicAuth else None
+            }
+            res = requests.post(url, headers=headers, json=batch)
+            if res.status_code != 200:
+                print("Error flushing log "+str(res.status_code))
+        except Exception as e:
+            print("Error flushing log "+str(e))
+
+
     def flushLoop(self):
         while True:
             with self.wait:
                 self.wait.wait(self.flushInterval/1000)
             batch = []
             while not self.buffer.empty():
                 batch.append(self.buffer.get())         
-            try:
-                url = self.options["baseUrl"]+"/api/"+self.options["org"]+"/"+self.options["stream"]+"/_json"   
-                basicAuth = self.options["auth"]
-                if not isinstance(basicAuth, str):
-                    if "username" in basicAuth and "password" in basicAuth:
-                        basicAuth = basicAuth["username"]+":"+basicAuth["password"]
-                        basicAuth = base64.b64encode(basicAuth.encode()).decode()
-                headers = {
-                    'Content-Type': 'application/json',
-                    "Authorization": "Basic "+basicAuth if basicAuth else None
-                }
-                res = requests.post(url, headers=headers, json=batch)
-                if res.status_code != 200:
-                    print("Error flushing log "+str(res.status_code))
-            except Exception as e:
-                print("Error flushing log "+str(e))
-
+            self._flushToOpenObserve(batch)
 
 
     
 
 
 class Logger :
     """
@@ -100,30 +114,30 @@
     - OPENOBSERVE_USERNAME: The username for basic authentication.
     - OPENOBSERVE_PASSWORD: The password for basic authentication.
     - OPENOBSERVE_BATCHSIZE: The batch size for logging to OpenObserve. Defaults to 21.
     - OPENOBSERVE_FLUSHINTERVAL: The flush interval for logging to OpenObserve. Defaults to 5000.
 
     """
 
-    def __init__(self, name:str, version:str, runner=None, level=None, enableOobs:bool=True):
+    def __init__(self, name:str, version:str, jobId:str=None, runnerLogger=None, level=None, enableOobs:bool=True):
         """
         Create a new logger.
         Args:
             name (str): The name of the logger.
             version (str): The version of the logger.
-            runner (object): The runner to log to. Defaults to None.
+            runnerLogger : The function to log to the runner.
             level (LogLevel): Optional: The minimum level of logs to print. Defaults to environment variable or "debug".
             enableOobs (bool): Optional: Whether to enable logging to OpenObserve. Defaults to True.
         """
         self.name=name or "main"
-        self.runner=runner
-        self.logger=None
+        self.runnerLogger=runnerLogger
         self.logLevel=None
         self.oobsLogger=None
         self.version=version
+        self.jobId=jobId
         
         logLevelName = os.getenv('LOG_LEVEL', "debug")
         oobsLogLevelName= os.getenv('OPENOBSERVE_LOGLEVEL', logLevelName)
 
         self.logLevel = self._levelToValue(logLevelName)
         self.oobsLogLevel = self._levelToValue(oobsLogLevelName)
         
@@ -143,15 +157,16 @@
                     "username": os.getenv('OPENOBSERVE_USERNAME', None),
                     "password": os.getenv('OPENOBSERVE_PASSWORD', None)
                 },
                 "batchSize": int(os.getenv('OPENOBSERVE_BATCHSIZE', 21)),
                 "flushInterval": int(os.getenv('OPENOBSERVE_FLUSHINTERVAL', 0)),
                 "meta":{
                     "appName": self.name,
-                    "appVersion": self.version
+                    "appVersion": self.version,
+                    "jobId": self.jobId
                 }                
             })
 
     def _levelToValue(self, level:LogLevel)->int:
         if level == "error": return 7
         if level == "warn": return 6
         if level == "info": return 5
@@ -167,21 +182,21 @@
         levelV=self._levelToValue(level)
         minLevel = self.logLevel
         minObsLevel = self.oobsLogLevel
         minNostrLevel = self._levelToValue("info")
 
         if levelV >= minLevel:
             date = time.strftime("%Y-%m-%d %H:%M:%S")
-            print(date+" ["+self.name+":"+self.version+"] : "+level+" : "+message)
+            print(date+" ["+self.name+":"+self.version+"] "+(("("+self.jobId+")") if self.jobId else "")+": "+level+" : "+message)
 
         if self.oobsLogger and levelV >= minObsLevel:
             self.oobsLogger.log(level, message)
         
-        if self.runner and levelV >= minNostrLevel:
-            self.runner._log(message)
+        if self.runnerLogger and levelV >= minNostrLevel:
+            self.runnerLogger(message)
 
 
     def log(self, *args):
         self._log("debug", args)
     
     def info(self, *args):
         self._log("info", args)
@@ -201,8 +216,13 @@
     
     def finer(self, *args):
         self._log("finer",  args)
 
     def finest(self, *args):
         self._log("finest", args)
 
+    def close(self):
+        if self.oobsLogger:
+            self.obsLogger.close()
+
+
```

### Comparing `openagents_node_sdk-0.1.5/openagents/OpenAgentsNode.py` & `openagents_node_sdk-0.2/openagents/OpenAgentsNode.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import os
 import traceback
 import asyncio
 from .JobRunner import JobRunner
 from .NodeConfig import NodeConfig
 from .Logger import Logger
 from typing import Union
-
+from .JobContext import JobContext
+import json
 class HeaderAdderInterceptor(grpc.aio.UnaryUnaryClientInterceptor):
     """
     An interceptor for GRPC that adds headers to outgoing requests.
     """
     def __init__(self, headers):
         self._headers = headers
 
@@ -38,62 +39,53 @@
     - POOL_ADDRESS: The address of the pool. Defaults to "
     - POOL_PORT: The port of the pool. Defaults to 5000.
     - POOL_SSL: Whether to use SSL for the pool. Defaults to False.
     - NODE_TPS: The ticks per second of the node main loop. Defaults to 10.
     - NODE_TOKEN: The token of the node. Defaults to None.
     """
   
-    def __init__(self, metaOrConfig: Union[dict, NodeConfig]):
-        meta=None
-        if isinstance(metaOrConfig, NodeConfig):
-            meta = metaOrConfig.getMeta()
-        else:
-            meta = metaOrConfig
-        self.nextNodeAnnounce = 0
-        self.nodeName = ""
-        self.nodeIcon = ""
-        self.nodeDescription = ""
+    def __init__(self, config: NodeConfig):
+        
+        self.meta = config.getMeta()
+            
+        self.nextNodeAnnounce = 0        
         self.channel = None
         self.rpcClient = None
-        self.runners=[]
+        self.registeredRunners=[]
         self.poolAddress = None
         self.poolPort = None
-        self.failedJobsTracker = []
+        self.lockedJobs = []
         self.isLooping = False
         self.logger = None
         self.loopInterval = 100
         
-        name = ""
-        icon = ""
-        description = ""
-        version = "0.0.1"
-
-        name = meta["name"] if "name" in meta else None
-        icon = meta["picture"] if "picture" in meta else None
-        description = meta["about"] if "about" in meta else None
-        version = meta["version"] if "version" in meta else None
-
-        self.nodeName = name or os.getenv('NODE_NAME', "OpenAgentsNode")
-        self.nodeIcon = icon or os.getenv('NODE_ICON', "")
-        self.nodeVersion = version or os.getenv('NODE_VERSION', "0.0.1")
-        self.nodeDescription = description or  os.getenv('NODE_DESCRIPTION', "")
+    
+        self.nodeName = self.meta["name"]
+        self.nodeIcon =  self.meta["picture"]
+        self.nodeVersion =  self.meta["version"]
+        self.nodeDescription =  self.meta["description"]
 
         self.channel = None
         self.rpcClient = None
         self.logger = Logger(self.nodeName,self.nodeVersion)
         self.logger.info("Starting "+self.nodeName+" v"+self.nodeVersion)
 
+    def getMeta(self):
+        return self.meta
+
     def registerRunner(self, runner:JobRunner) -> None:
         """
         Register a runner to the node.
         Args:
             runner (JobRunner): The runner to register.
         """
-        runner.logger=Logger(self.nodeName+"."+runner.__class__.__name__,self.nodeVersion,runner)
-        self.runners.append(runner)
+        self.registeredRunners.append({
+            "runner": runner,
+            "nextAnnouncementTimestamp": 0    
+        })
 
     def getLogger(self):
         """
         Get the active logger for the node.
         """
         return self.logger        
 
@@ -169,81 +161,96 @@
 
     async def _executePendingJobForRunner(self , runner:JobRunner):
         """
         Execute all pending jobs for a runner.
         Args:
             runner (JobRunner): The runner to execute the job.
         """
-        if runner not in self.runners:
+        if len([x for x in self.registeredRunners if x["runner"]==runner])==0:
             del self.runnerTasks[runner]
             return
+        
         try:
+            if not runner.initialized:
+                runner.initialized=True
+                await runner.init(self)
             client = self._getClient()
-            #for runner in self.runners:
             jobs=[]
-            for filter in runner._filters:
-                jobs.extend((await client.getPendingJobs(rpc_pb2.RpcGetPendingJobs(
-                    filterByRunOn =  filter["filterByRunOn"] if "filterByRunOn" in filter else None,
-                    filterByCustomer = filter["filterByCustomer"] if "filterByCustomer" in filter else None,
-                    filterByDescription = filter["filterByDescription"] if "filterByDescription" in filter else None,
-                    filterById = filter["filterById"] if "filterById" in filter else None,
-                    filterByKind  = filter["filterByKind"] if "filterByKind" in filter else None,
-                    wait=60000,
-                    # exclude failed jobs
-                    excludeId = [x[0] for x in self.failedJobsTracker if time.time()-x[1] < 60]
-                ))).jobs)    
+            filter = runner.getFilter()
+            self.lockedJobs = [x for x in self.lockedJobs if time.time()-x[1] < 60]
+            jobs.extend((await client.getPendingJobs(rpc_pb2.RpcGetPendingJobs(
+                filterByRunOn =  filter["filterByRunOn"] if "filterByRunOn" in filter else None,
+                filterByCustomer = filter["filterByCustomer"] if "filterByCustomer" in filter else None,
+                filterByDescription = filter["filterByDescription"] if "filterByDescription" in filter else None,
+                filterById = filter["filterById"] if "filterById" in filter else None,
+                filterByKind  = filter["filterByKind"] if "filterByKind" in filter else None,
+                wait=60000,
+                # exclude failed jobs
+                excludeId = [x[0] for x in self.lockedJobs]
+            ))).jobs)    
+
+            if len(jobs)>0 : self.getLogger().log(str(len(jobs))+" pending jobs for "+runner.__class__.__name__)
+            else : self.getLogger().finer("No pending jobs for "+runner.__class__.__name__)
             
-            for job in jobs:           
-                if len(jobs)>0 : runner.getLogger().log(str(len(jobs))+" pending jobs")
-                else : runner.getLogger().log("No pending jobs")
+            for job in jobs:              
                 wasAccepted=False
                 t=time.time()   
+                ctx = JobContext(self,runner,job)
                 try:
-                    client = self._getClient() # Reconnect client for each job
-                    if not await runner.canRun(job):
+                    client = self._getClient() # Refresh client connection if needed
+                    if not await runner.canRun(ctx):
+                        await ctx.close()
                         continue
+                    self.lockedJobs.append([job.id, time.time()])
                     await self._acceptJob(job.id)
                     wasAccepted = True
-                    runner.getLogger().info("Job started on node "+self.nodeName)  
-                    runner._setNode(self)
-                    runner._setJob(job)
-                    await runner.preRun(job)
+
+
+                    
+                    ctx.getLogger().info("Job started on node "+self.nodeName)  
+                    
+                    await runner.preRun(ctx)
                     async def task():
                         try:
-                            output=await runner.run(job)    
-                            await runner.postRun(job)                            
-                            runner.getLogger().info("Job completed in "+str(time.time()-t)+" seconds on node "+self.nodeName, job.id)                
+                            output=await runner.run(ctx) 
+                            await runner.postRun(ctx)                  
+                            ctx.getLogger().info("Job completed in "+str(time.time()-t)+" seconds on node "+self.nodeName, job.id)                
                             await client.completeJob(rpc_pb2.RpcJobOutput(jobId=job.id, output=output))
                         except Exception as e:
-                            self.failedJobsTracker.append([job.id, time.time()])
-                            runner.getLogger().error("Job failed in "+str(time.time()-t)+" seconds on node "+self.nodeName+" with error "+str(e), job.id)
+                            ctx.getLogger().error("Job failed in "+str(time.time()-t)+" seconds on node "+self.nodeName+" with error "+str(e), job.id)
                             if wasAccepted:
                                 await client.cancelJob(rpc_pb2.RpcCancelJob(jobId=job.id, reason=str(e)))
                             traceback.print_exc()
-                    asyncio.create_task(task())
+                        await ctx.close()
+                    if not runner.isRunInParallel():
+                        await task()
+                    else:
+                        asyncio.create_task(task())
                 except Exception as e:
-                    self.failedJobsTracker.append([job.id, time.time()])
-                    runner.getLogger().error("Job failed in "+str(time.time()-t)+" seconds on node "+self.nodeName+" with error "+str(e), job.id)
+                    ctx.getLogger().error("Job failed in "+str(time.time()-t)+" seconds on node "+self.nodeName+" with error "+str(e), job.id)
+                    await ctx.close()
                     if wasAccepted:
                         await client.cancelJob(rpc_pb2.RpcCancelJob(jobId=job.id, reason=str(e)))
                     traceback.print_exc()
+
         except Exception as e:
             traceback.print_exc()
-            runner.getLogger().error("Error executing runner "+str(e))
+            self.getLogger().error("Error executing runner "+str(e))
             await asyncio.sleep(5000.0/1000.0)
         self.runnerTasks[runner]=asyncio.create_task(self._executePendingJobForRunner(runner))
 
  
     runnerTasks={}
     async def _executePendingJob(self ):
         """
         Execute all pending jobs for all runners.
         """
-        for runner in self.runners:
+        for reg in self.registeredRunners:
             try:
+                runner = reg["runner"]
                 if not runner in self.runnerTasks:
                     self.runnerTasks[runner]=asyncio.create_task(self._executePendingJobForRunner(runner))
             except Exception as e:
                 self.getLogger().log("Error executing pending job "+str(e), None)
 
 
     async def reannounce(self):    
@@ -263,38 +270,38 @@
                     ))
                     self.nextNodeAnnounce = int(time.time()*1000) + res.refreshInterval
                     self.getLogger().log("Node announced, next announcement in "+str(res.refreshInterval)+" ms")
                 except Exception as e:
                     self.getLogger().error("Error announcing node "+ str(e), None)
                     self.nextNodeAnnounce = int(time.time()*1000) + 5000
 
-            for runner in self.runners:
+            for reg in self.registeredRunners:
                 try:
-                    if time_ms >= runner._nextAnnouncementTimestamp:
+                    if time_ms >=  reg["nextAnnouncementTimestamp"]:
                         client = self._getClient()
                         res = await client.announceEventTemplate(rpc_pb2.RpcAnnounceTemplateRequest(
-                            meta=runner._meta,
-                            template=runner._template,
-                            sockets=runner._sockets
+                            meta=json.dumps(reg["runner"].getMeta()),
+                            template=reg["runner"].getTemplate(),
+                            sockets=json.dumps(reg["runner"].getSockets())
                         ))
-                        runner._nextAnnouncementTimestamp = int(time.time()*1000) + res.refreshInterval
+                        reg["nextAnnouncementTimestamp"] = int(time.time()*1000) + res.refreshInterval
                         self.getLogger().log("Template announced, next announcement in "+str(res.refreshInterval)+" ms")
                 except Exception as e:
                     self.getLogger().error("Error announcing template "+ str(e), None)
-                    runner._nextAnnouncementTimestamp = int(time.time()*1000) + 5000
+                    reg["nextAnnouncementTimestamp"] = int(time.time()*1000) + 5000
         except Exception as e:
             self.getLogger().error("Error reannouncing "+str(e), None)
         await asyncio.sleep(5000.0/1000.0)
         asyncio.create_task(self.reannounce())
   
     async def _loop(self):
         """
         The main loop of the node.
         """
-        promises = [runner.loop() for runner in self.runners]
+        promises = [reg["runner"].loop(self) for reg in self.registeredRunners]
         await asyncio.gather(*promises)
         self.isLooping = False
         await asyncio.sleep(self.loopInterval/1000.0)
         asyncio.create_task(self._loop())
         
 
     async def _run(self, poolAddress=None, poolPort=None, poolSsl=False):
```

### Comparing `openagents_node_sdk-0.1.5/setup.py` & `openagents_node_sdk-0.2/setup.py`

 * *Files identical despite different names*

