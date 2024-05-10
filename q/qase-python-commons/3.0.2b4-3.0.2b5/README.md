# Comparing `tmp/qase_python_commons-3.0.2b4.tar.gz` & `tmp/qase_python_commons-3.0.2b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase_python_commons-3.0.2b4.tar", last modified: Tue May  7 18:05:34 2024, max compression
+gzip compressed data, was "qase_python_commons-3.0.2b5.tar", last modified: Thu May  9 08:49:33 2024, max compression
```

## Comparing `qase_python_commons-3.0.2b4.tar` & `qase_python_commons-3.0.2b5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:05:34.110403 qase_python_commons-3.0.2b4/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-07 18:05:34.110403 qase_python_commons-3.0.2b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 18:05:34.110403 qase_python_commons-3.0.2b4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:05:34.102403 qase_python_commons-3.0.2b4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:05:34.098403 qase_python_commons-3.0.2b4/src/qase/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:05:34.102403 qase_python_commons-3.0.2b4/src/qase/commons/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:05:34.102403 qase_python_commons-3.0.2b4/src/qase/commons/client/
--rw-r--r--   0 runner    (1001) docker     (127)    10934 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/client/api_v1_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/client/api_v2_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/client/base_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:05:34.102403 qase_python_commons-3.0.2b4/src/qase/commons/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/exceptions/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:05:34.106403 qase_python_commons-3.0.2b4/src/qase/commons/models/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/models/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/models/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/models/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/models/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/models/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/models/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/models/suite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:05:34.106403 qase_python_commons-3.0.2b4/src/qase/commons/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/profilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/profilers/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/profilers/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/profilers/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:05:34.106403 qase_python_commons-3.0.2b4/src/qase/commons/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/reporters/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/reporters/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/reporters/testops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:05:34.106403 qase_python_commons-3.0.2b4/src/qase/commons/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-07 18:05:27.000000 qase_python_commons-3.0.2b4/src/qase/commons/validators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:05:34.106403 qase_python_commons-3.0.2b4/src/qase_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-07 18:05:34.000000 qase_python_commons-3.0.2b4/src/qase_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-07 18:05:34.000000 qase_python_commons-3.0.2b4/src/qase_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:05:34.000000 qase_python_commons-3.0.2b4/src/qase_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-07 18:05:34.000000 qase_python_commons-3.0.2b4/src/qase_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 18:05:34.000000 qase_python_commons-3.0.2b4/src/qase_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:49:33.353580 qase_python_commons-3.0.2b5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-09 08:49:33.353580 qase_python_commons-3.0.2b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 08:49:33.353580 qase_python_commons-3.0.2b5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:49:33.345580 qase_python_commons-3.0.2b5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:49:33.345580 qase_python_commons-3.0.2b5/src/qase/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:49:33.349580 qase_python_commons-3.0.2b5/src/qase/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:49:33.349580 qase_python_commons-3.0.2b5/src/qase/commons/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10934 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/client/api_v1_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/client/api_v2_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/client/base_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:49:33.349580 qase_python_commons-3.0.2b5/src/qase/commons/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/exceptions/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:49:33.349580 qase_python_commons-3.0.2b5/src/qase/commons/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/models/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/models/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/models/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/models/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/models/suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:49:33.353580 qase_python_commons-3.0.2b5/src/qase/commons/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/profilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/profilers/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/profilers/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/profilers/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:49:33.353580 qase_python_commons-3.0.2b5/src/qase/commons/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/reporters/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/reporters/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/reporters/testops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:49:33.353580 qase_python_commons-3.0.2b5/src/qase/commons/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-09 08:49:26.000000 qase_python_commons-3.0.2b5/src/qase/commons/validators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:49:33.353580 qase_python_commons-3.0.2b5/src/qase_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-09 08:49:33.000000 qase_python_commons-3.0.2b5/src/qase_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-09 08:49:33.000000 qase_python_commons-3.0.2b5/src/qase_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 08:49:33.000000 qase_python_commons-3.0.2b5/src/qase_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-09 08:49:33.000000 qase_python_commons-3.0.2b5/src/qase_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 08:49:33.000000 qase_python_commons-3.0.2b5/src/qase_python_commons.egg-info/top_level.txt
```

### Comparing `qase_python_commons-3.0.2b4/PKG-INFO` & `qase_python_commons-3.0.2b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 3.0.2b4
+Version: 3.0.2b5
 Summary: A library for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `qase_python_commons-3.0.2b4/pyproject.toml` & `qase_python_commons-3.0.2b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-python-commons"
-version = "3.0.2b4"
+version = "3.0.2b5"
 description = "A library for Qase TestOps and Qase Report"
 readme = "README.md"
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
```

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/client/api_v1_client.py` & `qase_python_commons-3.0.2b5/src/qase/commons/client/api_v1_client.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/client/api_v2_client.py` & `qase_python_commons-3.0.2b5/src/qase/commons/client/api_v2_client.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/client/base_api_client.py` & `qase_python_commons-3.0.2b5/src/qase/commons/client/base_api_client.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/config.py` & `qase_python_commons-3.0.2b5/src/qase/commons/config.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/loader.py` & `qase_python_commons-3.0.2b5/src/qase/commons/loader.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/logger.py` & `qase_python_commons-3.0.2b5/src/qase/commons/logger.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/models/attachment.py` & `qase_python_commons-3.0.2b5/src/qase/commons/models/attachment.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/models/result.py` & `qase_python_commons-3.0.2b5/src/qase/commons/models/result.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/models/run.py` & `qase_python_commons-3.0.2b5/src/qase/commons/models/run.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/models/runtime.py` & `qase_python_commons-3.0.2b5/src/qase/commons/models/runtime.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/models/step.py` & `qase_python_commons-3.0.2b5/src/qase/commons/models/step.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/profilers/network.py` & `qase_python_commons-3.0.2b5/src/qase/commons/profilers/network.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from ..models.runtime import Runtime
 from ..models.step import Step, StepRequestData, StepType
 
 
 class NetworkProfiler:
     _instance = None
 
-    def __init__(self, runtime: Runtime, track_on_fail: bool = True):
+    def __init__(self, runtime: Runtime, skip_domain: str, track_on_fail: bool = True):
         self._original_functions = {}
         self.runtime = runtime
+        self.skip_domain = skip_domain
         self.track_on_fail = track_on_fail
         self.step = None
 
     def enable(self):
         if 'requests' in sys.modules:
             import requests
             self._original_functions['requests'] = requests.Session.send
@@ -33,54 +34,68 @@
         if 'urllib3' in self._original_functions:
             import urllib3
             urllib3.PoolManager.request = self._original_functions['urllib3']
 
     def _requests_send_wrapper(self, func):
         @wraps(func)
         def wrapper(self, request, *args, **kwargs):
-            NetworkProfilerSingleton.get_instance()._log_pre_request(request)
+            NetworkProfilerSingleton.get_instance()._log_request(request)
             response = func(self, request, *args, **kwargs)
-            NetworkProfilerSingleton.get_instance()._log_post_response(response)
+            NetworkProfilerSingleton.get_instance()._log_response(response)
             return response
 
         return wrapper
 
     def _urllib3_request_wrapper(self, func):
+        skip_domain = self.skip_domain
+
         @wraps(func)
         def wrapper(self, method, url, *args, **kwargs):
+            if skip_domain in url:
+                return func(self, method, url, *args, **kwargs)
+
             interceptor = NetworkProfilerSingleton.get_instance()
             request = lambda: None
             request.method = method
             request.url = url
 
-            interceptor._log_pre_request(request)
+            interceptor._log_request(request)
             response = func(self, method, url, *args, **kwargs)
-            if response is not None and interceptor.track_on_fail and response.status >= 400:
-                interceptor._log_post_response(response, url=url)
+            interceptor._log_response(response, url=url)
             return response
 
         return wrapper
 
     @staticmethod
-    def _log_pre_request(request):
+    def _log_request(request):
         NetworkProfilerSingleton.get_instance().step = Step(
             id=str(uuid.uuid4()),
             step_type=StepType.REQUEST,
             data=StepRequestData(
                 request_method=request.method,
                 request_url=request.url,
-                request_body=request.body,
-                request_headers=request.headers,
+                request_body=request.body if hasattr(request, 'body') else None,
+                request_headers=request.headers if hasattr(request, 'headers') else None
             ),
         )
 
     @staticmethod
-    def _log_post_response(response, url=None, *args, **kwargs):
+    def _log_response(response, url=None, *args, **kwargs):
         status = response.status if hasattr(response, 'status') else response.status_code
         profiler = NetworkProfilerSingleton.get_instance()
+        if profiler.step is None:
+            profiler.step = Step(
+                id=str(uuid.uuid4()),
+                step_type=StepType.REQUEST,
+                data=StepRequestData(
+                    request_method=response.request.method,
+                    request_url=response.request.url,
+                    request_body=response.request.body if hasattr(response.request, 'body') else None,
+                    request_headers=response.request.headers if hasattr(response.request, 'headers') else None
+                ))
         profiler.step.data.add_response(
             status_code=status,
             response_body=str(response.data if hasattr(response,
                                                        'data') else response.content) if profiler.track_on_fail and status >= 400 else None,
             response_headers=response.headers if profiler.track_on_fail and status >= 400 else None,
         )
         profiler.runtime.add_step(profiler.step)
```

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/profilers/sleep.py` & `qase_python_commons-3.0.2b5/src/qase/commons/profilers/sleep.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/reporters/core.py` & `qase_python_commons-3.0.2b5/src/qase/commons/reporters/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,16 @@
     def setup_profilers(self, runtime: Runtime) -> None:
         profilers = self.config.get("profilers", [])
 
         for profiler in profilers:
             if profiler == "network":
                 # Lazy import
                 from ..profilers import NetworkProfilerSingleton
-                NetworkProfilerSingleton.init(runtime=runtime)
+                NetworkProfilerSingleton.init(runtime=runtime,
+                                              skip_domain=self.config.get("testops.api.host", "qase.io"))
                 self.profilers.append(NetworkProfilerSingleton.get_instance())
             if profiler == "sleep":
                 from ..profilers import SleepProfiler
                 self.profilers.append(SleepProfiler(runtime=runtime))
             if profiler == "db":
                 from ..profilers import DbProfiler
                 self.profilers.append(DbProfiler(runtime=runtime))
```

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/reporters/report.py` & `qase_python_commons-3.0.2b5/src/qase/commons/reporters/report.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/reporters/testops.py` & `qase_python_commons-3.0.2b5/src/qase/commons/reporters/testops.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b4/src/qase/commons/utils.py` & `qase_python_commons-3.0.2b5/src/qase/commons/utils.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b4/src/qase_python_commons.egg-info/PKG-INFO` & `qase_python_commons-3.0.2b5/src/qase_python_commons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 3.0.2b4
+Version: 3.0.2b5
 Summary: A library for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `qase_python_commons-3.0.2b4/src/qase_python_commons.egg-info/SOURCES.txt` & `qase_python_commons-3.0.2b5/src/qase_python_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

