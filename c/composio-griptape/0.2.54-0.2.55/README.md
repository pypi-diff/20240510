# Comparing `tmp/composio_griptape-0.2.54.tar.gz` & `tmp/composio_griptape-0.2.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_griptape-0.2.54.tar", last modified: Fri May 10 09:57:21 2024, max compression
+gzip compressed data, was "composio_griptape-0.2.55.tar", last modified: Fri May 10 10:04:28 2024, max compression
```

## Comparing `composio_griptape-0.2.54.tar` & `composio_griptape-0.2.55.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-10 09:57:21.414108 composio_griptape-0.2.54/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2389 2024-05-10 09:57:21.413913 composio_griptape-0.2.54/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1851 2024-05-09 11:39:51.000000 composio_griptape-0.2.54/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-10 09:57:21.412776 composio_griptape-0.2.54/composio_griptape/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      161 2024-05-09 11:39:51.000000 composio_griptape-0.2.54/composio_griptape/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     5393 2024-05-09 11:39:51.000000 composio_griptape-0.2.54/composio_griptape/griptape_toolspec.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-10 09:57:21.413732 composio_griptape-0.2.54/composio_griptape.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2389 2024-05-10 09:57:21.000000 composio_griptape-0.2.54/composio_griptape.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      291 2024-05-10 09:57:21.000000 composio_griptape-0.2.54/composio_griptape.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-05-10 09:57:21.000000 composio_griptape-0.2.54/composio_griptape.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       40 2024-05-10 09:57:21.000000 composio_griptape-0.2.54/composio_griptape.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       18 2024-05-10 09:57:21.000000 composio_griptape-0.2.54/composio_griptape.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-05-10 09:57:21.414221 composio_griptape-0.2.54/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      853 2024-05-10 09:56:59.000000 composio_griptape-0.2.54/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-10 10:04:28.886897 composio_griptape-0.2.55/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2389 2024-05-10 10:04:28.886702 composio_griptape-0.2.55/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1851 2024-05-09 11:39:51.000000 composio_griptape-0.2.55/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-10 10:04:28.885524 composio_griptape-0.2.55/composio_griptape/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      161 2024-05-09 11:39:51.000000 composio_griptape-0.2.55/composio_griptape/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     5393 2024-05-09 11:39:51.000000 composio_griptape-0.2.55/composio_griptape/griptape_toolspec.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-10 10:04:28.886494 composio_griptape-0.2.55/composio_griptape.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2389 2024-05-10 10:04:28.000000 composio_griptape-0.2.55/composio_griptape.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      291 2024-05-10 10:04:28.000000 composio_griptape-0.2.55/composio_griptape.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-05-10 10:04:28.000000 composio_griptape-0.2.55/composio_griptape.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       40 2024-05-10 10:04:28.000000 composio_griptape-0.2.55/composio_griptape.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       18 2024-05-10 10:04:28.000000 composio_griptape-0.2.55/composio_griptape.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-05-10 10:04:28.886935 composio_griptape-0.2.55/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      853 2024-05-10 10:04:05.000000 composio_griptape-0.2.55/setup.py
```

### Comparing `composio_griptape-0.2.54/PKG-INFO` & `composio_griptape-0.2.55/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_griptape
-Version: 0.2.54
+Version: 0.2.55
 Summary: Use Composio to get an array of tools with your Griptape wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.49
+Requires-Dist: composio_core===0.2.55
 Requires-Dist: griptape>=0.24.2
 
 ## 🚀🔗 Integrating Composio with Griptape
 
 Streamline the integration of Composio within the Griptape agentic framework to enhance the interaction capabilities of Griptape agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_griptape-0.2.54/README.md` & `composio_griptape-0.2.55/README.md`

 * *Files identical despite different names*

### Comparing `composio_griptape-0.2.54/composio_griptape/griptape_toolspec.py` & `composio_griptape-0.2.55/composio_griptape/griptape_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_griptape-0.2.54/composio_griptape.egg-info/PKG-INFO` & `composio_griptape-0.2.55/composio_griptape.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_griptape
-Version: 0.2.54
+Version: 0.2.55
 Summary: Use Composio to get an array of tools with your Griptape wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.49
+Requires-Dist: composio_core===0.2.55
 Requires-Dist: griptape>=0.24.2
 
 ## 🚀🔗 Integrating Composio with Griptape
 
 Streamline the integration of Composio within the Griptape agentic framework to enhance the interaction capabilities of Griptape agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_griptape-0.2.54/setup.py` & `composio_griptape-0.2.55/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_griptape",
-    version="0.2.54",
+    version="0.2.55",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Griptape wokflow.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
     install_requires=[
-        "composio_core===0.2.49",
+        "composio_core===0.2.55",
         "griptape>=0.24.2"
     ],
     include_package_data=True,
 )
```

