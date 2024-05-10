# Comparing `tmp/pulumi_kafka-3.8.0a1715245833.tar.gz` & `tmp/pulumi_kafka-3.8.0a1715267369.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kafka-3.8.0a1715245833.tar", last modified: Thu May  9 09:15:05 2024, max compression
+gzip compressed data, was "pulumi_kafka-3.8.0a1715267369.tar", last modified: Thu May  9 15:11:44 2024, max compression
```

## Comparing `pulumi_kafka-3.8.0a1715245833.tar` & `pulumi_kafka-3.8.0a1715267369.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:15:05.651787 pulumi_kafka-3.8.0a1715245833/
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-09 09:15:05.651787 pulumi_kafka-3.8.0a1715245833/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-09 09:14:58.000000 pulumi_kafka-3.8.0a1715245833/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:15:05.651787 pulumi_kafka-3.8.0a1715245833/pulumi_kafka/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-09 09:14:58.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 09:14:58.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    23117 2024-05-09 09:14:58.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka/acl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:15:05.651787 pulumi_kafka-3.8.0a1715245833/pulumi_kafka/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 09:14:58.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-09 09:14:58.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-09 09:14:58.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-09 09:14:58.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka/get_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    31331 2024-05-09 09:14:58.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-09 09:14:58.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:14:58.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-05-09 09:14:58.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka/quota.py
--rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-05-09 09:14:58.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-05-09 09:14:58.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka/user_scram_credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:15:05.651787 pulumi_kafka-3.8.0a1715245833/pulumi_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-09 09:15:05.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-09 09:15:05.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:15:05.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 09:15:05.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 09:15:05.000000 pulumi_kafka-3.8.0a1715245833/pulumi_kafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-09 09:14:58.000000 pulumi_kafka-3.8.0a1715245833/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 09:15:05.651787 pulumi_kafka-3.8.0a1715245833/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:11:44.465421 pulumi_kafka-3.8.0a1715267369/
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-09 15:11:44.465421 pulumi_kafka-3.8.0a1715267369/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-09 15:11:38.000000 pulumi_kafka-3.8.0a1715267369/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:11:44.461420 pulumi_kafka-3.8.0a1715267369/pulumi_kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-09 15:11:38.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 15:11:38.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23117 2024-05-09 15:11:38.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka/acl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:11:44.465421 pulumi_kafka-3.8.0a1715267369/pulumi_kafka/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 15:11:38.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-09 15:11:38.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-09 15:11:38.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-09 15:11:38.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka/get_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31331 2024-05-09 15:11:38.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-09 15:11:38.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:11:38.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-05-09 15:11:38.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka/quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-05-09 15:11:38.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-05-09 15:11:38.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka/user_scram_credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:11:44.465421 pulumi_kafka-3.8.0a1715267369/pulumi_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-09 15:11:44.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-09 15:11:44.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:11:44.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 15:11:44.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 15:11:44.000000 pulumi_kafka-3.8.0a1715267369/pulumi_kafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-09 15:11:38.000000 pulumi_kafka-3.8.0a1715267369/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 15:11:44.465421 pulumi_kafka-3.8.0a1715267369/setup.cfg
```

### Comparing `pulumi_kafka-3.8.0a1715245833/PKG-INFO` & `pulumi_kafka-3.8.0a1715267369/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kafka
-Version: 3.8.0a1715245833
+Version: 3.8.0a1715267369
 Summary: A Pulumi package for creating and managing Kafka.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kafka
 Keywords: pulumi,kafka
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kafka-3.8.0a1715245833/README.md` & `pulumi_kafka-3.8.0a1715267369/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715245833/pulumi_kafka/__init__.py` & `pulumi_kafka-3.8.0a1715267369/pulumi_kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715245833/pulumi_kafka/_utilities.py` & `pulumi_kafka-3.8.0a1715267369/pulumi_kafka/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715245833/pulumi_kafka/acl.py` & `pulumi_kafka-3.8.0a1715267369/pulumi_kafka/acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715245833/pulumi_kafka/config/__init__.pyi` & `pulumi_kafka-3.8.0a1715267369/pulumi_kafka/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715245833/pulumi_kafka/config/vars.py` & `pulumi_kafka-3.8.0a1715267369/pulumi_kafka/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715245833/pulumi_kafka/get_topic.py` & `pulumi_kafka-3.8.0a1715267369/pulumi_kafka/get_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715245833/pulumi_kafka/provider.py` & `pulumi_kafka-3.8.0a1715267369/pulumi_kafka/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715245833/pulumi_kafka/quota.py` & `pulumi_kafka-3.8.0a1715267369/pulumi_kafka/quota.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715245833/pulumi_kafka/topic.py` & `pulumi_kafka-3.8.0a1715267369/pulumi_kafka/topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715245833/pulumi_kafka/user_scram_credential.py` & `pulumi_kafka-3.8.0a1715267369/pulumi_kafka/user_scram_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715245833/pulumi_kafka.egg-info/PKG-INFO` & `pulumi_kafka-3.8.0a1715267369/pulumi_kafka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kafka
-Version: 3.8.0a1715245833
+Version: 3.8.0a1715267369
 Summary: A Pulumi package for creating and managing Kafka.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kafka
 Keywords: pulumi,kafka
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kafka-3.8.0a1715245833/pulumi_kafka.egg-info/SOURCES.txt` & `pulumi_kafka-3.8.0a1715267369/pulumi_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715245833/pyproject.toml` & `pulumi_kafka-3.8.0a1715267369/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kafka"
   description = "A Pulumi package for creating and managing Kafka."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "kafka"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.8.0a1715245833"
+  version = "3.8.0a1715267369"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-kafka"
 
 [build-system]
```

