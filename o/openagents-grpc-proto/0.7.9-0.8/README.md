# Comparing `tmp/openagents_grpc_proto-0.7.9.tar.gz` & `tmp/openagents_grpc_proto-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openagents_grpc_proto-0.7.9.tar", last modified: Sat May  4 08:44:17 2024, max compression
+gzip compressed data, was "openagents_grpc_proto-0.8.tar", last modified: Fri May 10 06:56:49 2024, max compression
```

## Comparing `openagents_grpc_proto-0.7.9.tar` & `openagents_grpc_proto-0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:44:17.920720 openagents_grpc_proto-0.7.9/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-04 08:44:17.920720 openagents_grpc_proto-0.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:44:17.916720 openagents_grpc_proto-0.7.9/openagents_grpc_proto/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobInput_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobParam_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobParam_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobResult_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobResult_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobState_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobState_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobStatus_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/Job_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/Job_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/Log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/Log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/rpc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    45184 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto/rpc_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:44:17.920720 openagents_grpc_proto-0.7.9/openagents_grpc_proto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/openagents_grpc_proto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 08:44:17.920720 openagents_grpc_proto-0.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-04 08:44:17.000000 openagents_grpc_proto-0.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:56:49.655357 openagents_grpc_proto-0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-10 06:56:49.655357 openagents_grpc_proto-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:56:49.655357 openagents_grpc_proto-0.8/openagents_grpc_proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/JobInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/JobInput_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/JobParam_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/JobParam_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/JobResult_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/JobResult_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/JobState_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/JobState_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/JobStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/JobStatus_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/Job_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/Job_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/Log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/Log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/rpc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53937 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto/rpc_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:56:49.655357 openagents_grpc_proto-0.8/openagents_grpc_proto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/openagents_grpc_proto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 06:56:49.655357 openagents_grpc_proto-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-10 06:56:49.000000 openagents_grpc_proto-0.8/setup.py
```

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobInput_pb2.py` & `openagents_grpc_proto-0.8/openagents_grpc_proto/JobInput_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobInput_pb2_grpc.py` & `openagents_grpc_proto-0.8/openagents_grpc_proto/JobInput_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobParam_pb2.py` & `openagents_grpc_proto-0.8/openagents_grpc_proto/JobParam_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobParam_pb2_grpc.py` & `openagents_grpc_proto-0.8/openagents_grpc_proto/JobParam_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobResult_pb2.py` & `openagents_grpc_proto-0.8/openagents_grpc_proto/JobResult_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobResult_pb2_grpc.py` & `openagents_grpc_proto-0.8/openagents_grpc_proto/JobResult_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobState_pb2.py` & `openagents_grpc_proto-0.8/openagents_grpc_proto/JobState_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobState_pb2_grpc.py` & `openagents_grpc_proto-0.8/openagents_grpc_proto/JobState_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobStatus_pb2.py` & `openagents_grpc_proto-0.8/openagents_grpc_proto/JobStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto/JobStatus_pb2_grpc.py` & `openagents_grpc_proto-0.8/openagents_grpc_proto/JobStatus_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto/Job_pb2.py` & `openagents_grpc_proto-0.8/openagents_grpc_proto/Job_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto/Job_pb2_grpc.py` & `openagents_grpc_proto-0.8/openagents_grpc_proto/Job_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto/Log_pb2.py` & `openagents_grpc_proto-0.8/openagents_grpc_proto/Log_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto/Log_pb2_grpc.py` & `openagents_grpc_proto-0.8/openagents_grpc_proto/Log_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto/rpc_pb2.py` & `openagents_grpc_proto-0.8/openagents_grpc_proto/rpc_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import JobState_pb2 as JobState__pb2
 import JobParam_pb2 as JobParam__pb2
 import JobInput_pb2 as JobInput__pb2
 import JobResult_pb2 as JobResult__pb2
 import Job_pb2 as Job__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\trpc.proto\x1a\tLog.proto\x1a\x0fJobStatus.proto\x1a\x0eJobState.proto\x1a\x0eJobParam.proto\x1a\x0eJobInput.proto\x1a\x0fJobResult.proto\x1a\tJob.proto\"\x9c\x02\n\rRpcRequestJob\x12\r\n\x05runOn\x18\x01 \x01(\t\x12\x13\n\x0b\x65xpireAfter\x18\x02 \x01(\x04\x12\x18\n\x05input\x18\x03 \x03(\x0b\x32\t.JobInput\x12\x18\n\x05param\x18\x04 \x03(\x0b\x32\t.JobParam\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x11\n\x04kind\x18\x07 \x01(\rH\x00\x88\x01\x01\x12\x19\n\x0coutputFormat\x18\x08 \x01(\tH\x01\x88\x01\x01\x12\x1c\n\x0frequestProvider\x18\t \x01(\tH\x02\x88\x01\x01\x12\x16\n\tencrypted\x18\n \x01(\x08H\x03\x88\x01\x01\x42\x07\n\x05_kindB\x0f\n\r_outputFormatB\x12\n\x10_requestProviderB\x0c\n\n_encrypted\"6\n\tRpcGetJob\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x63 \x01(\rH\x00\x88\x01\x01\x42\x07\n\x05_wait\"\xb2\x02\n\x11RpcGetPendingJobs\x12\x1a\n\rfilterByRunOn\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x1d\n\x10\x66ilterByCustomer\x18\x02 \x01(\tH\x01\x88\x01\x01\x12 \n\x13\x66ilterByDescription\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x17\n\nfilterById\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x19\n\x0c\x66ilterByKind\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x11\n\texcludeId\x18\x62 \x03(\t\x12\x11\n\x04wait\x18\x63 \x01(\rH\x05\x88\x01\x01\x42\x10\n\x0e_filterByRunOnB\x13\n\x11_filterByCustomerB\x16\n\x14_filterByDescriptionB\r\n\x0b_filterByIdB\x0f\n\r_filterByKindB\x07\n\x05_wait\"!\n\x0bPendingJobs\x12\x12\n\x04jobs\x18\x01 \x03(\x0b\x32\x04.Job\"\x1e\n\x0cRpcIsJobDone\x12\x0e\n\x06isDone\x18\x01 \x01(\x08\"\x1d\n\x0cRpcAcceptJob\x12\r\n\x05jobId\x18\x01 \x01(\t\"-\n\x0cRpcCancelJob\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"-\n\x0cRpcJobOutput\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x0e\n\x06output\x18\x02 \x01(\t\"K\n\x0eRpcJobComplete\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x0e\n\x06output\x18\x02 \x01(\t\x12\x11\n\x04info\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x07\n\x05_info\"\'\n\tRpcJobLog\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x0b\n\x03log\x18\x02 \x01(\t\";\n\x19RpcSendSignedEventRequest\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\r\n\x05\x65vent\x18\x02 \x01(\t\"?\n\x1bRpcSubscribeToEventsRequest\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x0f\n\x07\x66ilters\x18\x02 \x03(\t\"G\n\x1cRpcSubscribeToEventsResponse\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x16\n\x0esubscriptionId\x18\x02 \x01(\t\"M\n\x13RpcGetEventsRequest\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x16\n\x0esubscriptionId\x18\x02 \x01(\t\x12\r\n\x05limit\x18\x03 \x01(\r\"^\n\x14RpcGetEventsResponse\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x16\n\x0esubscriptionId\x18\x03 \x01(\t\x12\x0e\n\x06\x65vents\x18\x04 \x03(\t\">\n\x1aRpcSendSignedEventResponse\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\"J\n\x1fRpcUnsubscribeFromEventsRequest\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x16\n\x0esubscriptionId\x18\x02 \x01(\t\"3\n RpcUnsubscribeFromEventsResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"L\n\x16RpcAnnounceNodeRequest\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\"C\n\x17RpcAnnounceNodeResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0frefreshInterval\x18\x04 \x01(\x04\"M\n\x1aRpcAnnounceTemplateRequest\x12\x0c\n\x04meta\x18\x01 \x01(\t\x12\x10\n\x08template\x18\x02 \x01(\t\x12\x0f\n\x07sockets\x18\x03 \x01(\t\"G\n\x1bRpcAnnounceTemplateResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0frefreshInterval\x18\x04 \x01(\x04\"\xa6\x01\n\x14RpcCreateDiskRequest\x12\x11\n\x04name\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x1a\n\rencryptionKey\x18\x02 \x01(\tH\x01\x88\x01\x01\x12&\n\x19includeEncryptionKeyInUrl\x18\x03 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_nameB\x10\n\x0e_encryptionKeyB\x1c\n\x1a_includeEncryptionKeyInUrl\"$\n\x15RpcCreateDiskResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\"O\n\x12RpcOpenDiskRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x1a\n\rencryptionKey\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x10\n\x0e_encryptionKey\"G\n\x13RpcOpenDiskResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x0e\n\x06\x64iskId\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x04\"%\n\x13RpcCloseDiskRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\"\'\n\x14RpcCloseDiskResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"8\n\x18RpcDiskDeleteFileRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\",\n\x19RpcDiskDeleteFileResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"7\n\x17RpcDiskListFilesRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\")\n\x18RpcDiskListFilesResponse\x12\r\n\x05\x66iles\x18\x01 \x03(\t\"6\n\x16RpcDiskReadFileRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"7\n\x17RpcDiskReadFileResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0e\n\x06\x65xists\x18\x02 \x01(\x08\"E\n\x17RpcDiskWriteFileRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"+\n\x18RpcDiskWriteFileResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"u\n\x12RpcCacheSetRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x14\n\x07version\x18\x03 \x01(\x04H\x00\x88\x01\x01\x12\x15\n\x08\x65xpireAt\x18\x04 \x01(\x04H\x01\x88\x01\x01\x42\n\n\x08_versionB\x0b\n\t_expireAt\"&\n\x13RpcCacheSetResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"K\n\x12RpcCacheGetRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x0blastVersion\x18\x02 \x01(\x04H\x00\x88\x01\x01\x42\x0e\n\x0c_lastVersion\"3\n\x13RpcCacheGetResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0e\n\x06\x65xists\x18\x02 \x01(\x08\x32\xf5\x0b\n\rPoolConnector\x12\"\n\nrequestJob\x12\x0e.RpcRequestJob\x1a\x04.Job\x12\x1a\n\x06getJob\x12\n.RpcGetJob\x1a\x04.Job\x12\x32\n\x0egetPendingJobs\x12\x12.RpcGetPendingJobs\x1a\x0c.PendingJobs\x12&\n\tisJobDone\x12\n.RpcGetJob\x1a\r.RpcIsJobDone\x12 \n\tacceptJob\x12\r.RpcAcceptJob\x1a\x04.Job\x12 \n\tcancelJob\x12\r.RpcCancelJob\x1a\x04.Job\x12#\n\x0coutputForJob\x12\r.RpcJobOutput\x1a\x04.Job\x12$\n\x0b\x63ompleteJob\x12\x0f.RpcJobComplete\x1a\x04.Job\x12\x1d\n\tlogForJob\x12\n.RpcJobLog\x1a\x04.Job\x12\x41\n\x0c\x61nnounceNode\x12\x17.RpcAnnounceNodeRequest\x1a\x18.RpcAnnounceNodeResponse\x12R\n\x15\x61nnounceEventTemplate\x12\x1b.RpcAnnounceTemplateRequest\x1a\x1c.RpcAnnounceTemplateResponse\x12J\n\x0fsendSignedEvent\x12\x1a.RpcSendSignedEventRequest\x1a\x1b.RpcSendSignedEventResponse\x12P\n\x11subscribeToEvents\x12\x1c.RpcSubscribeToEventsRequest\x1a\x1d.RpcSubscribeToEventsResponse\x12\\\n\x15unsubscribeFromEvents\x12 .RpcUnsubscribeFromEventsRequest\x1a!.RpcUnsubscribeFromEventsResponse\x12\x38\n\tgetEvents\x12\x14.RpcGetEventsRequest\x1a\x15.RpcGetEventsResponse\x12;\n\ncreateDisk\x12\x15.RpcCreateDiskRequest\x1a\x16.RpcCreateDiskResponse\x12\x35\n\x08openDisk\x12\x13.RpcOpenDiskRequest\x1a\x14.RpcOpenDiskResponse\x12\x38\n\tcloseDisk\x12\x14.RpcCloseDiskRequest\x1a\x15.RpcCloseDiskResponse\x12G\n\x0e\x64iskDeleteFile\x12\x19.RpcDiskDeleteFileRequest\x1a\x1a.RpcDiskDeleteFileResponse\x12\x44\n\rdiskListFiles\x12\x18.RpcDiskListFilesRequest\x1a\x19.RpcDiskListFilesResponse\x12\x43\n\x0c\x64iskReadFile\x12\x17.RpcDiskReadFileRequest\x1a\x18.RpcDiskReadFileResponse0\x01\x12\x46\n\x11\x64iskReadSmallFile\x12\x17.RpcDiskReadFileRequest\x1a\x18.RpcDiskReadFileResponse\x12\x46\n\rdiskWriteFile\x12\x18.RpcDiskWriteFileRequest\x1a\x19.RpcDiskWriteFileResponse(\x01\x12I\n\x12\x64iskWriteSmallFile\x12\x18.RpcDiskWriteFileRequest\x1a\x19.RpcDiskWriteFileResponse\x12\x37\n\x08\x63\x61\x63heSet\x12\x13.RpcCacheSetRequest\x1a\x14.RpcCacheSetResponse(\x01\x12\x37\n\x08\x63\x61\x63heGet\x12\x13.RpcCacheGetRequest\x1a\x14.RpcCacheGetResponse0\x01\x42.\xca\x02\x0e\x41pp\\Grpc\\nostr\xe2\x02\x1a\x41pp\\Grpc\\nostr\\GPBMetadatab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\trpc.proto\x1a\tLog.proto\x1a\x0fJobStatus.proto\x1a\x0eJobState.proto\x1a\x0eJobParam.proto\x1a\x0eJobInput.proto\x1a\x0fJobResult.proto\x1a\tJob.proto\"\x9c\x02\n\rRpcRequestJob\x12\r\n\x05runOn\x18\x01 \x01(\t\x12\x13\n\x0b\x65xpireAfter\x18\x02 \x01(\x04\x12\x18\n\x05input\x18\x03 \x03(\x0b\x32\t.JobInput\x12\x18\n\x05param\x18\x04 \x03(\x0b\x32\t.JobParam\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x11\n\x04kind\x18\x07 \x01(\rH\x00\x88\x01\x01\x12\x19\n\x0coutputFormat\x18\x08 \x01(\tH\x01\x88\x01\x01\x12\x1c\n\x0frequestProvider\x18\t \x01(\tH\x02\x88\x01\x01\x12\x16\n\tencrypted\x18\n \x01(\x08H\x03\x88\x01\x01\x42\x07\n\x05_kindB\x0f\n\r_outputFormatB\x12\n\x10_requestProviderB\x0c\n\n_encrypted\"6\n\tRpcGetJob\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x63 \x01(\rH\x00\x88\x01\x01\x42\x07\n\x05_wait\"\xb2\x02\n\x11RpcGetPendingJobs\x12\x1a\n\rfilterByRunOn\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x1d\n\x10\x66ilterByCustomer\x18\x02 \x01(\tH\x01\x88\x01\x01\x12 \n\x13\x66ilterByDescription\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x17\n\nfilterById\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x19\n\x0c\x66ilterByKind\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x11\n\texcludeId\x18\x62 \x03(\t\x12\x11\n\x04wait\x18\x63 \x01(\rH\x05\x88\x01\x01\x42\x10\n\x0e_filterByRunOnB\x13\n\x11_filterByCustomerB\x16\n\x14_filterByDescriptionB\r\n\x0b_filterByIdB\x0f\n\r_filterByKindB\x07\n\x05_wait\"!\n\x0bPendingJobs\x12\x12\n\x04jobs\x18\x01 \x03(\x0b\x32\x04.Job\"\x1e\n\x0cRpcIsJobDone\x12\x0e\n\x06isDone\x18\x01 \x01(\x08\"\x1d\n\x0cRpcAcceptJob\x12\r\n\x05jobId\x18\x01 \x01(\t\"-\n\x0cRpcCancelJob\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"-\n\x0cRpcJobOutput\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x0e\n\x06output\x18\x02 \x01(\t\"K\n\x0eRpcJobComplete\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x0e\n\x06output\x18\x02 \x01(\t\x12\x11\n\x04info\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x07\n\x05_info\"\'\n\tRpcJobLog\x12\r\n\x05jobId\x18\x01 \x01(\t\x12\x0b\n\x03log\x18\x02 \x01(\t\";\n\x19RpcSendSignedEventRequest\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\r\n\x05\x65vent\x18\x02 \x01(\t\"?\n\x1bRpcSubscribeToEventsRequest\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x0f\n\x07\x66ilters\x18\x02 \x03(\t\"G\n\x1cRpcSubscribeToEventsResponse\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x16\n\x0esubscriptionId\x18\x02 \x01(\t\"M\n\x13RpcGetEventsRequest\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x16\n\x0esubscriptionId\x18\x02 \x01(\t\x12\r\n\x05limit\x18\x03 \x01(\r\"^\n\x14RpcGetEventsResponse\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\x16\n\x0esubscriptionId\x18\x03 \x01(\t\x12\x0e\n\x06\x65vents\x18\x04 \x03(\t\">\n\x1aRpcSendSignedEventResponse\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\"J\n\x1fRpcUnsubscribeFromEventsRequest\x12\x0f\n\x07groupId\x18\x01 \x01(\t\x12\x16\n\x0esubscriptionId\x18\x02 \x01(\t\"3\n RpcUnsubscribeFromEventsResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"L\n\x16RpcAnnounceNodeRequest\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\"C\n\x17RpcAnnounceNodeResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0frefreshInterval\x18\x04 \x01(\x04\"M\n\x1aRpcAnnounceTemplateRequest\x12\x0c\n\x04meta\x18\x01 \x01(\t\x12\x10\n\x08template\x18\x02 \x01(\t\x12\x0f\n\x07sockets\x18\x03 \x01(\t\"G\n\x1bRpcAnnounceTemplateResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0frefreshInterval\x18\x04 \x01(\x04\"\xa6\x01\n\x14RpcCreateDiskRequest\x12\x11\n\x04name\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x1a\n\rencryptionKey\x18\x02 \x01(\tH\x01\x88\x01\x01\x12&\n\x19includeEncryptionKeyInUrl\x18\x03 \x01(\x08H\x02\x88\x01\x01\x42\x07\n\x05_nameB\x10\n\x0e_encryptionKeyB\x1c\n\x1a_includeEncryptionKeyInUrl\"$\n\x15RpcCreateDiskResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\"O\n\x12RpcOpenDiskRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x1a\n\rencryptionKey\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x10\n\x0e_encryptionKey\"G\n\x13RpcOpenDiskResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x0e\n\x06\x64iskId\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x04\"%\n\x13RpcCloseDiskRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\"\'\n\x14RpcCloseDiskResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"8\n\x18RpcDiskDeleteFileRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\",\n\x19RpcDiskDeleteFileResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"7\n\x17RpcDiskListFilesRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\")\n\x18RpcDiskListFilesResponse\x12\r\n\x05\x66iles\x18\x01 \x03(\t\"6\n\x16RpcDiskReadFileRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"7\n\x17RpcDiskReadFileResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0e\n\x06\x65xists\x18\x02 \x01(\x08\"E\n\x17RpcDiskWriteFileRequest\x12\x0e\n\x06\x64iskId\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"+\n\x18RpcDiskWriteFileResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"u\n\x12RpcCacheSetRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x14\n\x07version\x18\x03 \x01(\x04H\x00\x88\x01\x01\x12\x15\n\x08\x65xpireAt\x18\x04 \x01(\x04H\x01\x88\x01\x01\x42\n\n\x08_versionB\x0b\n\t_expireAt\"&\n\x13RpcCacheSetResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"K\n\x12RpcCacheGetRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x0blastVersion\x18\x02 \x01(\x04H\x00\x88\x01\x01\x42\x0e\n\x0c_lastVersion\"3\n\x13RpcCacheGetResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0e\n\x06\x65xists\x18\x02 \x01(\x08\"\x19\n\x17RpcDiscoverPoolsRequest\")\n\x18RpcDiscoverPoolsResponse\x12\r\n\x05pools\x18\x01 \x03(\t\"^\n\x17RpcDiscoverNodesRequest\x12\x15\n\rfilterByKinds\x18\x01 \x03(\x05\x12\x15\n\rfilterByPools\x18\x02 \x03(\t\x12\x15\n\rfilterByNodes\x18\x03 \x03(\t\")\n\x18RpcDiscoverNodesResponse\x12\r\n\x05nodes\x18\x01 \x03(\t\"v\n\x19RpcDiscoverActionsRequest\x12\x15\n\rfilterByKinds\x18\x01 \x03(\x05\x12\x15\n\rfilterByPools\x18\x02 \x03(\t\x12\x15\n\rfilterByNodes\x18\x03 \x03(\t\x12\x14\n\x0c\x66ilterByTags\x18\x04 \x03(\t\"-\n\x1aRpcDiscoverActionsResponse\x12\x0f\n\x07\x61\x63tions\x18\x01 \x03(\t\"M\n\x1dRpcDiscoverNearbyNodesRequest\x12\x15\n\rfilterByKinds\x18\x01 \x03(\x05\x12\x15\n\rfilterByNodes\x18\x03 \x03(\t\"/\n\x1eRpcDiscoverNearbyNodesResponse\x12\r\n\x05nodes\x18\x01 \x03(\t\"e\n\x1fRpcDiscoverNearbyActionsRequest\x12\x15\n\rfilterByKinds\x18\x01 \x03(\x05\x12\x15\n\rfilterByNodes\x18\x03 \x03(\t\x12\x14\n\x0c\x66ilterByTags\x18\x04 \x03(\t\"3\n RpcDiscoverNearbyActionsResponse\x12\x0f\n\x07\x61\x63tions\x18\x01 \x03(\t2\x83\x0f\n\rPoolConnector\x12\"\n\nrequestJob\x12\x0e.RpcRequestJob\x1a\x04.Job\x12\x1a\n\x06getJob\x12\n.RpcGetJob\x1a\x04.Job\x12\x32\n\x0egetPendingJobs\x12\x12.RpcGetPendingJobs\x1a\x0c.PendingJobs\x12&\n\tisJobDone\x12\n.RpcGetJob\x1a\r.RpcIsJobDone\x12 \n\tacceptJob\x12\r.RpcAcceptJob\x1a\x04.Job\x12 \n\tcancelJob\x12\r.RpcCancelJob\x1a\x04.Job\x12#\n\x0coutputForJob\x12\r.RpcJobOutput\x1a\x04.Job\x12$\n\x0b\x63ompleteJob\x12\x0f.RpcJobComplete\x1a\x04.Job\x12\x1d\n\tlogForJob\x12\n.RpcJobLog\x1a\x04.Job\x12\x41\n\x0c\x61nnounceNode\x12\x17.RpcAnnounceNodeRequest\x1a\x18.RpcAnnounceNodeResponse\x12R\n\x15\x61nnounceEventTemplate\x12\x1b.RpcAnnounceTemplateRequest\x1a\x1c.RpcAnnounceTemplateResponse\x12\x44\n\rdiscoverPools\x12\x18.RpcDiscoverPoolsRequest\x1a\x19.RpcDiscoverPoolsResponse\x12\x44\n\rdiscoverNodes\x12\x18.RpcDiscoverNodesRequest\x1a\x19.RpcDiscoverNodesResponse\x12J\n\x0f\x64iscoverActions\x12\x1a.RpcDiscoverActionsRequest\x1a\x1b.RpcDiscoverActionsResponse\x12V\n\x13\x64iscoverNearbyNodes\x12\x1e.RpcDiscoverNearbyNodesRequest\x1a\x1f.RpcDiscoverNearbyNodesResponse\x12\\\n\x15\x64iscoverNearbyActions\x12 .RpcDiscoverNearbyActionsRequest\x1a!.RpcDiscoverNearbyActionsResponse\x12J\n\x0fsendSignedEvent\x12\x1a.RpcSendSignedEventRequest\x1a\x1b.RpcSendSignedEventResponse\x12P\n\x11subscribeToEvents\x12\x1c.RpcSubscribeToEventsRequest\x1a\x1d.RpcSubscribeToEventsResponse\x12\\\n\x15unsubscribeFromEvents\x12 .RpcUnsubscribeFromEventsRequest\x1a!.RpcUnsubscribeFromEventsResponse\x12\x38\n\tgetEvents\x12\x14.RpcGetEventsRequest\x1a\x15.RpcGetEventsResponse\x12;\n\ncreateDisk\x12\x15.RpcCreateDiskRequest\x1a\x16.RpcCreateDiskResponse\x12\x35\n\x08openDisk\x12\x13.RpcOpenDiskRequest\x1a\x14.RpcOpenDiskResponse\x12\x38\n\tcloseDisk\x12\x14.RpcCloseDiskRequest\x1a\x15.RpcCloseDiskResponse\x12G\n\x0e\x64iskDeleteFile\x12\x19.RpcDiskDeleteFileRequest\x1a\x1a.RpcDiskDeleteFileResponse\x12\x44\n\rdiskListFiles\x12\x18.RpcDiskListFilesRequest\x1a\x19.RpcDiskListFilesResponse\x12\x43\n\x0c\x64iskReadFile\x12\x17.RpcDiskReadFileRequest\x1a\x18.RpcDiskReadFileResponse0\x01\x12\x46\n\x11\x64iskReadSmallFile\x12\x17.RpcDiskReadFileRequest\x1a\x18.RpcDiskReadFileResponse\x12\x46\n\rdiskWriteFile\x12\x18.RpcDiskWriteFileRequest\x1a\x19.RpcDiskWriteFileResponse(\x01\x12I\n\x12\x64iskWriteSmallFile\x12\x18.RpcDiskWriteFileRequest\x1a\x19.RpcDiskWriteFileResponse\x12\x37\n\x08\x63\x61\x63heSet\x12\x13.RpcCacheSetRequest\x1a\x14.RpcCacheSetResponse(\x01\x12\x37\n\x08\x63\x61\x63heGet\x12\x13.RpcCacheGetRequest\x1a\x14.RpcCacheGetResponse0\x01\x42.\xca\x02\x0e\x41pp\\Grpc\\nostr\xe2\x02\x1a\x41pp\\Grpc\\nostr\\GPBMetadatab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'rpc_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
   _globals['DESCRIPTOR']._serialized_options = b'\312\002\016App\\Grpc\\nostr\342\002\032App\\Grpc\\nostr\\GPBMetadata'
@@ -105,10 +105,30 @@
   _globals['_RPCCACHESETREQUEST']._serialized_end=2936
   _globals['_RPCCACHESETRESPONSE']._serialized_start=2938
   _globals['_RPCCACHESETRESPONSE']._serialized_end=2976
   _globals['_RPCCACHEGETREQUEST']._serialized_start=2978
   _globals['_RPCCACHEGETREQUEST']._serialized_end=3053
   _globals['_RPCCACHEGETRESPONSE']._serialized_start=3055
   _globals['_RPCCACHEGETRESPONSE']._serialized_end=3106
-  _globals['_POOLCONNECTOR']._serialized_start=3109
-  _globals['_POOLCONNECTOR']._serialized_end=4634
+  _globals['_RPCDISCOVERPOOLSREQUEST']._serialized_start=3108
+  _globals['_RPCDISCOVERPOOLSREQUEST']._serialized_end=3133
+  _globals['_RPCDISCOVERPOOLSRESPONSE']._serialized_start=3135
+  _globals['_RPCDISCOVERPOOLSRESPONSE']._serialized_end=3176
+  _globals['_RPCDISCOVERNODESREQUEST']._serialized_start=3178
+  _globals['_RPCDISCOVERNODESREQUEST']._serialized_end=3272
+  _globals['_RPCDISCOVERNODESRESPONSE']._serialized_start=3274
+  _globals['_RPCDISCOVERNODESRESPONSE']._serialized_end=3315
+  _globals['_RPCDISCOVERACTIONSREQUEST']._serialized_start=3317
+  _globals['_RPCDISCOVERACTIONSREQUEST']._serialized_end=3435
+  _globals['_RPCDISCOVERACTIONSRESPONSE']._serialized_start=3437
+  _globals['_RPCDISCOVERACTIONSRESPONSE']._serialized_end=3482
+  _globals['_RPCDISCOVERNEARBYNODESREQUEST']._serialized_start=3484
+  _globals['_RPCDISCOVERNEARBYNODESREQUEST']._serialized_end=3561
+  _globals['_RPCDISCOVERNEARBYNODESRESPONSE']._serialized_start=3563
+  _globals['_RPCDISCOVERNEARBYNODESRESPONSE']._serialized_end=3610
+  _globals['_RPCDISCOVERNEARBYACTIONSREQUEST']._serialized_start=3612
+  _globals['_RPCDISCOVERNEARBYACTIONSREQUEST']._serialized_end=3713
+  _globals['_RPCDISCOVERNEARBYACTIONSRESPONSE']._serialized_start=3715
+  _globals['_RPCDISCOVERNEARBYACTIONSRESPONSE']._serialized_end=3766
+  _globals['_POOLCONNECTOR']._serialized_start=3769
+  _globals['_POOLCONNECTOR']._serialized_end=5692
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto/rpc_pb2_grpc.py` & `openagents_grpc_proto-0.8/openagents_grpc_proto/rpc_pb2_grpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -91,14 +91,39 @@
                 response_deserializer=rpc__pb2.RpcAnnounceNodeResponse.FromString,
                 _registered_method=True)
         self.announceEventTemplate = channel.unary_unary(
                 '/PoolConnector/announceEventTemplate',
                 request_serializer=rpc__pb2.RpcAnnounceTemplateRequest.SerializeToString,
                 response_deserializer=rpc__pb2.RpcAnnounceTemplateResponse.FromString,
                 _registered_method=True)
+        self.discoverPools = channel.unary_unary(
+                '/PoolConnector/discoverPools',
+                request_serializer=rpc__pb2.RpcDiscoverPoolsRequest.SerializeToString,
+                response_deserializer=rpc__pb2.RpcDiscoverPoolsResponse.FromString,
+                _registered_method=True)
+        self.discoverNodes = channel.unary_unary(
+                '/PoolConnector/discoverNodes',
+                request_serializer=rpc__pb2.RpcDiscoverNodesRequest.SerializeToString,
+                response_deserializer=rpc__pb2.RpcDiscoverNodesResponse.FromString,
+                _registered_method=True)
+        self.discoverActions = channel.unary_unary(
+                '/PoolConnector/discoverActions',
+                request_serializer=rpc__pb2.RpcDiscoverActionsRequest.SerializeToString,
+                response_deserializer=rpc__pb2.RpcDiscoverActionsResponse.FromString,
+                _registered_method=True)
+        self.discoverNearbyNodes = channel.unary_unary(
+                '/PoolConnector/discoverNearbyNodes',
+                request_serializer=rpc__pb2.RpcDiscoverNearbyNodesRequest.SerializeToString,
+                response_deserializer=rpc__pb2.RpcDiscoverNearbyNodesResponse.FromString,
+                _registered_method=True)
+        self.discoverNearbyActions = channel.unary_unary(
+                '/PoolConnector/discoverNearbyActions',
+                request_serializer=rpc__pb2.RpcDiscoverNearbyActionsRequest.SerializeToString,
+                response_deserializer=rpc__pb2.RpcDiscoverNearbyActionsResponse.FromString,
+                _registered_method=True)
         self.sendSignedEvent = channel.unary_unary(
                 '/PoolConnector/sendSignedEvent',
                 request_serializer=rpc__pb2.RpcSendSignedEventRequest.SerializeToString,
                 response_deserializer=rpc__pb2.RpcSendSignedEventResponse.FromString,
                 _registered_method=True)
         self.subscribeToEvents = channel.unary_unary(
                 '/PoolConnector/subscribeToEvents',
@@ -239,14 +264,44 @@
 
     def announceEventTemplate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def discoverPools(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def discoverNodes(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def discoverActions(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def discoverNearbyNodes(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def discoverNearbyActions(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def sendSignedEvent(self, request, context):
         """generic nostr events
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -390,14 +445,39 @@
                     response_serializer=rpc__pb2.RpcAnnounceNodeResponse.SerializeToString,
             ),
             'announceEventTemplate': grpc.unary_unary_rpc_method_handler(
                     servicer.announceEventTemplate,
                     request_deserializer=rpc__pb2.RpcAnnounceTemplateRequest.FromString,
                     response_serializer=rpc__pb2.RpcAnnounceTemplateResponse.SerializeToString,
             ),
+            'discoverPools': grpc.unary_unary_rpc_method_handler(
+                    servicer.discoverPools,
+                    request_deserializer=rpc__pb2.RpcDiscoverPoolsRequest.FromString,
+                    response_serializer=rpc__pb2.RpcDiscoverPoolsResponse.SerializeToString,
+            ),
+            'discoverNodes': grpc.unary_unary_rpc_method_handler(
+                    servicer.discoverNodes,
+                    request_deserializer=rpc__pb2.RpcDiscoverNodesRequest.FromString,
+                    response_serializer=rpc__pb2.RpcDiscoverNodesResponse.SerializeToString,
+            ),
+            'discoverActions': grpc.unary_unary_rpc_method_handler(
+                    servicer.discoverActions,
+                    request_deserializer=rpc__pb2.RpcDiscoverActionsRequest.FromString,
+                    response_serializer=rpc__pb2.RpcDiscoverActionsResponse.SerializeToString,
+            ),
+            'discoverNearbyNodes': grpc.unary_unary_rpc_method_handler(
+                    servicer.discoverNearbyNodes,
+                    request_deserializer=rpc__pb2.RpcDiscoverNearbyNodesRequest.FromString,
+                    response_serializer=rpc__pb2.RpcDiscoverNearbyNodesResponse.SerializeToString,
+            ),
+            'discoverNearbyActions': grpc.unary_unary_rpc_method_handler(
+                    servicer.discoverNearbyActions,
+                    request_deserializer=rpc__pb2.RpcDiscoverNearbyActionsRequest.FromString,
+                    response_serializer=rpc__pb2.RpcDiscoverNearbyActionsResponse.SerializeToString,
+            ),
             'sendSignedEvent': grpc.unary_unary_rpc_method_handler(
                     servicer.sendSignedEvent,
                     request_deserializer=rpc__pb2.RpcSendSignedEventRequest.FromString,
                     response_serializer=rpc__pb2.RpcSendSignedEventResponse.SerializeToString,
             ),
             'subscribeToEvents': grpc.unary_unary_rpc_method_handler(
                     servicer.subscribeToEvents,
@@ -769,14 +849,149 @@
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
+            metadata,
+            _registered_method=True)
+
+    @staticmethod
+    def discoverPools(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/PoolConnector/discoverPools',
+            rpc__pb2.RpcDiscoverPoolsRequest.SerializeToString,
+            rpc__pb2.RpcDiscoverPoolsResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
+
+    @staticmethod
+    def discoverNodes(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/PoolConnector/discoverNodes',
+            rpc__pb2.RpcDiscoverNodesRequest.SerializeToString,
+            rpc__pb2.RpcDiscoverNodesResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
+
+    @staticmethod
+    def discoverActions(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/PoolConnector/discoverActions',
+            rpc__pb2.RpcDiscoverActionsRequest.SerializeToString,
+            rpc__pb2.RpcDiscoverActionsResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
+
+    @staticmethod
+    def discoverNearbyNodes(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/PoolConnector/discoverNearbyNodes',
+            rpc__pb2.RpcDiscoverNearbyNodesRequest.SerializeToString,
+            rpc__pb2.RpcDiscoverNearbyNodesResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
+
+    @staticmethod
+    def discoverNearbyActions(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/PoolConnector/discoverNearbyActions',
+            rpc__pb2.RpcDiscoverNearbyActionsRequest.SerializeToString,
+            rpc__pb2.RpcDiscoverNearbyActionsResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
             metadata,
             _registered_method=True)
 
     @staticmethod
     def sendSignedEvent(request,
             target,
             options=(),
```

### Comparing `openagents_grpc_proto-0.7.9/openagents_grpc_proto.egg-info/SOURCES.txt` & `openagents_grpc_proto-0.8/openagents_grpc_proto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

