# Comparing `tmp/openagents_node_sdk-0.2.tar.gz` & `tmp/openagents_node_sdk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openagents_node_sdk-0.2.tar", last modified: Fri May 10 07:00:01 2024, max compression
+gzip compressed data, was "openagents_node_sdk-0.2.1.tar", last modified: Fri May 10 12:14:03 2024, max compression
```

## Comparing `openagents_node_sdk-0.2.tar` & `openagents_node_sdk-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:00:01.548777 openagents_node_sdk-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-10 07:00:01.548777 openagents_node_sdk-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:00:01.548777 openagents_node_sdk-0.2/openagents/
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/Disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/DiskReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/DiskWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/JobContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/JobRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/NodeConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/OpenAgentsNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/RunnerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/openagents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:00:01.548777 openagents_node_sdk-0.2/openagents_node_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-10 07:00:01.000000 openagents_node_sdk-0.2/openagents_node_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-10 07:00:01.000000 openagents_node_sdk-0.2/openagents_node_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:00:01.000000 openagents_node_sdk-0.2/openagents_node_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 07:00:01.000000 openagents_node_sdk-0.2/openagents_node_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 07:00:01.000000 openagents_node_sdk-0.2/openagents_node_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 07:00:01.548777 openagents_node_sdk-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-10 06:59:58.000000 openagents_node_sdk-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:14:03.633315 openagents_node_sdk-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-10 12:14:01.000000 openagents_node_sdk-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 12:14:01.000000 openagents_node_sdk-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-10 12:14:03.633315 openagents_node_sdk-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-10 12:14:01.000000 openagents_node_sdk-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 12:14:01.000000 openagents_node_sdk-0.2.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:14:03.633315 openagents_node_sdk-0.2.1/openagents/
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-10 12:14:01.000000 openagents_node_sdk-0.2.1/openagents/Disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-10 12:14:01.000000 openagents_node_sdk-0.2.1/openagents/DiskReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-10 12:14:01.000000 openagents_node_sdk-0.2.1/openagents/DiskWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-05-10 12:14:01.000000 openagents_node_sdk-0.2.1/openagents/JobContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-10 12:14:01.000000 openagents_node_sdk-0.2.1/openagents/JobRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-05-10 12:14:01.000000 openagents_node_sdk-0.2.1/openagents/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-10 12:14:01.000000 openagents_node_sdk-0.2.1/openagents/NodeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-05-10 12:14:01.000000 openagents_node_sdk-0.2.1/openagents/OpenAgentsNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-10 12:14:01.000000 openagents_node_sdk-0.2.1/openagents/RunnerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-10 12:14:01.000000 openagents_node_sdk-0.2.1/openagents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:14:03.633315 openagents_node_sdk-0.2.1/openagents_node_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-10 12:14:03.000000 openagents_node_sdk-0.2.1/openagents_node_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-10 12:14:03.000000 openagents_node_sdk-0.2.1/openagents_node_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:14:03.000000 openagents_node_sdk-0.2.1/openagents_node_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 12:14:03.000000 openagents_node_sdk-0.2.1/openagents_node_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 12:14:03.000000 openagents_node_sdk-0.2.1/openagents_node_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:14:03.633315 openagents_node_sdk-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-10 12:14:01.000000 openagents_node_sdk-0.2.1/setup.py
```

### Comparing `openagents_node_sdk-0.2/LICENSE` & `openagents_node_sdk-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.2/README.md` & `openagents_node_sdk-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.2/openagents/Disk.py` & `openagents_node_sdk-0.2.1/openagents/Disk.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.2/openagents/DiskReader.py` & `openagents_node_sdk-0.2.1/openagents/DiskReader.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.2/openagents/DiskWriter.py` & `openagents_node_sdk-0.2.1/openagents/DiskWriter.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.2/openagents/JobContext.py` & `openagents_node_sdk-0.2.1/openagents/JobContext.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.2/openagents/JobRunner.py` & `openagents_node_sdk-0.2.1/openagents/JobRunner.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.2/openagents/Logger.py` & `openagents_node_sdk-0.2.1/openagents/Logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,11 +218,11 @@
         self._log("finer",  args)
 
     def finest(self, *args):
         self._log("finest", args)
 
     def close(self):
         if self.oobsLogger:
-            self.obsLogger.close()
+            self.oobsLogger.close()
```

### Comparing `openagents_node_sdk-0.2/openagents/NodeConfig.py` & `openagents_node_sdk-0.2.1/openagents/NodeConfig.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.2/openagents/OpenAgentsNode.py` & `openagents_node_sdk-0.2.1/openagents/OpenAgentsNode.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.2/openagents/RunnerConfig.py` & `openagents_node_sdk-0.2.1/openagents/RunnerConfig.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.2/setup.py` & `openagents_node_sdk-0.2.1/setup.py`

 * *Files identical despite different names*

