# Comparing `tmp/composio_openai-0.2.52.tar.gz` & `tmp/composio_openai-0.2.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_openai-0.2.52.tar", last modified: Tue May  7 09:18:48 2024, max compression
+gzip compressed data, was "composio_openai-0.2.55.tar", last modified: Fri May 10 10:04:47 2024, max compression
```

## Comparing `composio_openai-0.2.52.tar` & `composio_openai-0.2.55.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-07 09:18:48.278505 composio_openai-0.2.52/
--rw-r--r--   0 sawradip   (501) staff       (20)     2615 2024-05-07 09:18:48.278313 composio_openai-0.2.52/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)     2107 2024-05-02 07:57:45.000000 composio_openai-0.2.52/README.md
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-07 09:18:48.276936 composio_openai-0.2.52/composio_openai/
--rw-r--r--   0 sawradip   (501) staff       (20)      182 2024-05-02 07:57:45.000000 composio_openai-0.2.52/composio_openai/__init__.py
--rw-r--r--   0 sawradip   (501) staff       (20)     3105 2024-05-07 08:56:06.000000 composio_openai-0.2.52/composio_openai/openai_toolspec.py
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-07 09:18:48.278087 composio_openai-0.2.52/composio_openai.egg-info/
--rw-r--r--   0 sawradip   (501) staff       (20)     2615 2024-05-07 09:18:48.000000 composio_openai-0.2.52/composio_openai.egg-info/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)      275 2024-05-07 09:18:48.000000 composio_openai-0.2.52/composio_openai.egg-info/SOURCES.txt
--rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-07 09:18:48.000000 composio_openai-0.2.52/composio_openai.egg-info/dependency_links.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       23 2024-05-07 09:18:48.000000 composio_openai-0.2.52/composio_openai.egg-info/requires.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       16 2024-05-07 09:18:48.000000 composio_openai-0.2.52/composio_openai.egg-info/top_level.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-07 09:18:48.278551 composio_openai-0.2.52/setup.cfg
--rw-r--r--   0 sawradip   (501) staff       (20)      826 2024-05-07 09:18:22.000000 composio_openai-0.2.52/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-10 10:04:47.859344 composio_openai-0.2.55/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2615 2024-05-10 10:04:47.859143 composio_openai-0.2.55/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2107 2024-05-09 11:39:51.000000 composio_openai-0.2.55/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-10 10:04:47.858031 composio_openai-0.2.55/composio_openai/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      182 2024-05-09 11:39:51.000000 composio_openai-0.2.55/composio_openai/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3105 2024-05-09 11:39:51.000000 composio_openai-0.2.55/composio_openai/openai_toolspec.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-10 10:04:47.858956 composio_openai-0.2.55/composio_openai.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2615 2024-05-10 10:04:47.000000 composio_openai-0.2.55/composio_openai.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      275 2024-05-10 10:04:47.000000 composio_openai-0.2.55/composio_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-05-10 10:04:47.000000 composio_openai-0.2.55/composio_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       23 2024-05-10 10:04:47.000000 composio_openai-0.2.55/composio_openai.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       16 2024-05-10 10:04:47.000000 composio_openai-0.2.55/composio_openai.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-05-10 10:04:47.859384 composio_openai-0.2.55/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      826 2024-05-10 10:04:05.000000 composio_openai-0.2.55/setup.py
```

### Comparing `composio_openai-0.2.52/PKG-INFO` & `composio_openai-0.2.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_openai
-Version: 0.2.52
+Version: 0.2.55
 Summary: Use Composio to get an array of tools with your OpenAI Function Call.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.52
+Requires-Dist: composio_core===0.2.55
 
 ## 🚀🔗 Leveraging OpenAI with Composio
 
 Facilitate the integration of OpenAI with Composio to empower OpenAI models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_openai-0.2.52/README.md` & `composio_openai-0.2.55/README.md`

 * *Files identical despite different names*

### Comparing `composio_openai-0.2.52/composio_openai/openai_toolspec.py` & `composio_openai-0.2.55/composio_openai/openai_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_openai-0.2.52/composio_openai.egg-info/PKG-INFO` & `composio_openai-0.2.55/composio_openai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_openai
-Version: 0.2.52
+Version: 0.2.55
 Summary: Use Composio to get an array of tools with your OpenAI Function Call.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.52
+Requires-Dist: composio_core===0.2.55
 
 ## 🚀🔗 Leveraging OpenAI with Composio
 
 Facilitate the integration of OpenAI with Composio to empower OpenAI models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_openai-0.2.52/setup.py` & `composio_openai-0.2.55/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_openai",
-    version="0.2.52",
+    version="0.2.55",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your OpenAI Function Call.",
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
-        "composio_core===0.2.52",
+        "composio_core===0.2.55",
     ],
     include_package_data=True,
 )
```

