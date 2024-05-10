# Comparing `tmp/robin_api-1.4.tar.gz` & `tmp/robin_api-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robin_api-1.4.tar", last modified: Tue May  7 04:56:04 2024, max compression
+gzip compressed data, was "robin_api-1.5.tar", last modified: Fri May 10 00:48:02 2024, max compression
```

## Comparing `robin_api-1.4.tar` & `robin_api-1.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-07 04:56:04.244107 robin_api-1.4/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    11337 2024-04-30 18:06:24.000000 robin_api-1.4/LICENSE
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      210 2024-05-01 19:41:22.000000 robin_api-1.4/MANIFEST.in
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    15167 2024-05-07 04:56:04.244107 robin_api-1.4/PKG-INFO
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    14720 2024-05-07 04:31:29.000000 robin_api-1.4/README.md
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-07 04:56:04.244107 robin_api-1.4/robin_api/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      765 2024-05-02 19:33:54.000000 robin_api-1.4/robin_api/__init__.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    12382 2024-05-07 02:08:18.000000 robin_api-1.4/robin_api/_client.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     5102 2024-04-30 23:37:44.000000 robin_api-1.4/robin_api/_compat.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      404 2024-04-30 23:05:14.000000 robin_api-1.4/robin_api/_constants.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     3573 2024-04-30 20:26:30.000000 robin_api-1.4/robin_api/_exceptions.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    18240 2024-05-01 18:18:56.000000 robin_api-1.4/robin_api/_models.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      951 2024-05-02 19:39:40.000000 robin_api-1.4/robin_api/_resource.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     7217 2024-04-30 23:44:46.000000 robin_api-1.4/robin_api/_streaming.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     9696 2024-04-30 23:36:19.000000 robin_api-1.4/robin_api/_types.py
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-07 04:56:04.244107 robin_api-1.4/robin_api/_utils/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      219 2024-05-01 02:38:52.000000 robin_api-1.4/robin_api/_utils/__init__.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1553 2024-05-01 02:38:37.000000 robin_api-1.4/robin_api/_utils/_utils.py
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-07 04:56:04.244107 robin_api-1.4/robin_api/resources/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      164 2024-05-06 00:49:45.000000 robin_api-1.4/robin_api/resources/__init__.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     5050 2024-05-07 03:00:16.000000 robin_api-1.4/robin_api/resources/completions.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     4260 2024-05-07 03:59:52.000000 robin_api-1.4/robin_api/resources/files.py
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-07 04:56:04.244107 robin_api-1.4/robin_api/types/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      853 2024-05-07 00:28:45.000000 robin_api-1.4/robin_api/types/__init__.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     2025 2024-05-06 00:21:01.000000 robin_api-1.4/robin_api/types/chat_completion.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     3783 2024-05-06 00:07:24.000000 robin_api-1.4/robin_api/types/chat_completion_chunk.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1241 2024-05-03 21:04:08.000000 robin_api-1.4/robin_api/types/chat_completion_message.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      866 2024-05-03 21:04:32.000000 robin_api-1.4/robin_api/types/chat_completion_message_tool_call.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1139 2024-05-01 16:49:41.000000 robin_api-1.4/robin_api/types/completion.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      928 2024-05-01 17:15:49.000000 robin_api-1.4/robin_api/types/completion_choice.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      401 2024-05-01 00:30:19.000000 robin_api-1.4/robin_api/types/completion_usage.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      285 2024-05-07 00:28:29.000000 robin_api-1.4/robin_api/types/models_robin.py
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-07 04:56:04.244107 robin_api-1.4/robin_api.egg-info/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      726 2024-05-07 04:56:04.000000 robin_api-1.4/robin_api.egg-info/SOURCES.txt
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)       38 2024-05-07 04:56:04.244107 robin_api-1.4/setup.cfg
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      725 2024-05-07 04:55:52.000000 robin_api-1.4/setup.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-10 00:48:02.245630 robin_api-1.5/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    11337 2024-04-30 18:06:24.000000 robin_api-1.5/LICENSE
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      210 2024-05-01 19:41:22.000000 robin_api-1.5/MANIFEST.in
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    17355 2024-05-10 00:48:02.245630 robin_api-1.5/PKG-INFO
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    16908 2024-05-10 00:44:24.000000 robin_api-1.5/README.md
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-10 00:48:02.241630 robin_api-1.5/robin_api/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      765 2024-05-02 19:33:54.000000 robin_api-1.5/robin_api/__init__.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    12382 2024-05-07 02:08:18.000000 robin_api-1.5/robin_api/_client.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     5102 2024-04-30 23:37:44.000000 robin_api-1.5/robin_api/_compat.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      404 2024-04-30 23:05:14.000000 robin_api-1.5/robin_api/_constants.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     3573 2024-04-30 20:26:30.000000 robin_api-1.5/robin_api/_exceptions.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    18240 2024-05-01 18:18:56.000000 robin_api-1.5/robin_api/_models.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      951 2024-05-02 19:39:40.000000 robin_api-1.5/robin_api/_resource.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     7217 2024-04-30 23:44:46.000000 robin_api-1.5/robin_api/_streaming.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     9696 2024-04-30 23:36:19.000000 robin_api-1.5/robin_api/_types.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-10 00:48:02.241630 robin_api-1.5/robin_api/_utils/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      219 2024-05-01 02:38:52.000000 robin_api-1.5/robin_api/_utils/__init__.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1553 2024-05-01 02:38:37.000000 robin_api-1.5/robin_api/_utils/_utils.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-10 00:48:02.245630 robin_api-1.5/robin_api/resources/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      164 2024-05-06 00:49:45.000000 robin_api-1.5/robin_api/resources/__init__.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     5050 2024-05-07 03:00:16.000000 robin_api-1.5/robin_api/resources/completions.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     5855 2024-05-09 20:27:08.000000 robin_api-1.5/robin_api/resources/files.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-10 00:48:02.245630 robin_api-1.5/robin_api/types/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      902 2024-05-09 04:13:37.000000 robin_api-1.5/robin_api/types/__init__.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     2025 2024-05-06 00:21:01.000000 robin_api-1.5/robin_api/types/chat_completion.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     3783 2024-05-06 00:07:24.000000 robin_api-1.5/robin_api/types/chat_completion_chunk.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1241 2024-05-03 21:04:08.000000 robin_api-1.5/robin_api/types/chat_completion_message.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      866 2024-05-03 21:04:32.000000 robin_api-1.5/robin_api/types/chat_completion_message_tool_call.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1139 2024-05-01 16:49:41.000000 robin_api-1.5/robin_api/types/completion.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      928 2024-05-01 17:15:49.000000 robin_api-1.5/robin_api/types/completion_choice.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      401 2024-05-01 00:30:19.000000 robin_api-1.5/robin_api/types/completion_usage.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      529 2024-05-09 20:21:50.000000 robin_api-1.5/robin_api/types/models_robin.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-10 00:48:02.245630 robin_api-1.5/robin_api.egg-info/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      726 2024-05-10 00:48:02.000000 robin_api-1.5/robin_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)       38 2024-05-10 00:48:02.245630 robin_api-1.5/setup.cfg
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      747 2024-05-10 00:47:51.000000 robin_api-1.5/setup.py
```

### Comparing `robin_api-1.4/LICENSE` & `robin_api-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/PKG-INFO` & `robin_api-1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin_api
-Version: 1.4
+Version: 1.5
 Summary: file
 Home-page: https://github.com/williamgomez71/RobinApi
 Author: William Gomez
 Author-email: william.gomez712@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -263,15 +263,70 @@
         "prompt_tokens": 2915,
         "total_tokens": 2991
     }
 }
 ```
 
 
+6. Upload Web Page information Function
+This function allows uploading information from a web page into the system, storing the relevant data in an organized structure for subsequent analysis and retrieva
+
+```python
+folder_information = client.files.upload_web_page_information(
+    url="https://web.com/example",
+    deep_level=1
+)
+
+folder_information = client.files.upload_web_page_information(
+    url="https://web.com/example",
+    deep_level=1,
+    folder_id="112ccd00-3814-4f1e-975d-adsflkj6l"
+)
+
+
+```
+**Parameters:**
+
+- **url**: The URL of the web page from which to extract information.
+
+- **deep_level** (optional): The depth level for data extraction. A higher value results in more exhaustive exploration.
+  - **Accepted Values**: `1`, `2`, `3`.
+  - **Default**: `1`.
+
+- **folder_id** (optional): The folder ID where the extracted information will be stored. If not specified, a new folder will be created.
+
+**Response Structure:**
+
+```python
+ApiResponse(
+    status_code=200,
+    message={
+        'folder': {
+            'apiFolderId': '112ccd00-3814-4f1e-975d-094974d2b89d',
+            'createdAt': '2024-05-09T20:26:55.000000Z'
+        },
+        'file': {
+            'url': 'https://platform.openai.com/docs/guides/fine-tuning/preparing-your-dataset',
+            'tokens': None,
+            'documentId': None,
+            'createdAt': '2024-05-09T20:29:12.000000Z'
+        }
+    }
+)
+```
 
 
+- **folder**: Contains details about the folder where the web page data is stored.
+  - **apiFolderId**: The unique identifier of the folder created or used for storing the extracted information.
+  - **createdAt**: The timestamp indicating when the folder was created, in ISO 8601 format.
+
+- **file**: Provides information about the extracted web page.
+  - **url**: The URL of the web page that was uploaded for data extraction.
+  - **tokens**: This field will be populated once the indexing process is complete, representing the total number of tokens extracted from the web page content.
+  - **documentId**: Will be created after indexing, serving as a unique identifier for the document.
+  - **createdAt**: The timestamp indicating when the file was created, in ISO 8601 format.
```

### Comparing `robin_api-1.4/README.md` & `robin_api-1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -247,13 +247,68 @@
         "prompt_tokens": 2915,
         "total_tokens": 2991
     }
 }
 ```
 
 
+6. Upload Web Page information Function
+This function allows uploading information from a web page into the system, storing the relevant data in an organized structure for subsequent analysis and retrieva
 
+```python
+folder_information = client.files.upload_web_page_information(
+    url="https://web.com/example",
+    deep_level=1
+)
+
+folder_information = client.files.upload_web_page_information(
+    url="https://web.com/example",
+    deep_level=1,
+    folder_id="112ccd00-3814-4f1e-975d-adsflkj6l"
+)
 
 
+```
+**Parameters:**
+
+- **url**: The URL of the web page from which to extract information.
+
+- **deep_level** (optional): The depth level for data extraction. A higher value results in more exhaustive exploration.
+  - **Accepted Values**: `1`, `2`, `3`.
+  - **Default**: `1`.
+
+- **folder_id** (optional): The folder ID where the extracted information will be stored. If not specified, a new folder will be created.
+
+**Response Structure:**
+
+```python
+ApiResponse(
+    status_code=200,
+    message={
+        'folder': {
+            'apiFolderId': '112ccd00-3814-4f1e-975d-094974d2b89d',
+            'createdAt': '2024-05-09T20:26:55.000000Z'
+        },
+        'file': {
+            'url': 'https://platform.openai.com/docs/guides/fine-tuning/preparing-your-dataset',
+            'tokens': None,
+            'documentId': None,
+            'createdAt': '2024-05-09T20:29:12.000000Z'
+        }
+    }
+)
+```
+
+
+- **folder**: Contains details about the folder where the web page data is stored.
+  - **apiFolderId**: The unique identifier of the folder created or used for storing the extracted information.
+  - **createdAt**: The timestamp indicating when the folder was created, in ISO 8601 format.
+
+- **file**: Provides information about the extracted web page.
+  - **url**: The URL of the web page that was uploaded for data extraction.
+  - **tokens**: This field will be populated once the indexing process is complete, representing the total number of tokens extracted from the web page content.
+  - **documentId**: Will be created after indexing, serving as a unique identifier for the document.
+  - **createdAt**: The timestamp indicating when the file was created, in ISO 8601 format.
+
```

### Comparing `robin_api-1.4/robin_api/__init__.py` & `robin_api-1.5/robin_api/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/robin_api/_client.py` & `robin_api-1.5/robin_api/_client.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/robin_api/_compat.py` & `robin_api-1.5/robin_api/_compat.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/robin_api/_exceptions.py` & `robin_api-1.5/robin_api/_exceptions.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/robin_api/_models.py` & `robin_api-1.5/robin_api/_models.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/robin_api/_resource.py` & `robin_api-1.5/robin_api/_resource.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/robin_api/_streaming.py` & `robin_api-1.5/robin_api/_streaming.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/robin_api/_types.py` & `robin_api-1.5/robin_api/_types.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/robin_api/_utils/_utils.py` & `robin_api-1.5/robin_api/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/robin_api/resources/completions.py` & `robin_api-1.5/robin_api/resources/completions.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/robin_api/types/__init__.py` & `robin_api-1.5/robin_api/types/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 from .chat_completion_chunk import ChoiceDelta as ChoiceDelta
 from .chat_completion_chunk import ChoiceDeltaFunctionCall as ChoiceDeltaFunctionCall
 from .chat_completion_chunk import ChoiceDeltaToolCall as ChoiceDeltaToolCall
 from .chat_completion_chunk import ChoiceDeltaToolCallFunction as ChoiceDeltaToolCallFunction
 from .chat_completion import ChatCompletion as ChatCompletion
 from .chat_completion import ApiResponse as ApiResponse
 from .models_robin import Models as Models
+from .models_robin import DeepLevel as DeepLevel
```

### Comparing `robin_api-1.4/robin_api/types/chat_completion.py` & `robin_api-1.5/robin_api/types/chat_completion.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/robin_api/types/chat_completion_chunk.py` & `robin_api-1.5/robin_api/types/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/robin_api/types/chat_completion_message.py` & `robin_api-1.5/robin_api/types/chat_completion_message.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/robin_api/types/chat_completion_message_tool_call.py` & `robin_api-1.5/robin_api/types/chat_completion_message_tool_call.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/robin_api/types/completion.py` & `robin_api-1.5/robin_api/types/completion.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/robin_api/types/completion_choice.py` & `robin_api-1.5/robin_api/types/completion_choice.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/robin_api.egg-info/SOURCES.txt` & `robin_api-1.5/robin_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robin_api-1.4/setup.py` & `robin_api-1.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 #packages=find_packages()
 #packages=['robin_api'],
 setup(
     name='robin_api',
-    version='1.4',
+    version='1.5',
     packages=find_packages(),
     description="file",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'httpx',
         'pydantic',
-        'distro'
+        'distro',
+        'validators'
     ],
     python_requires='>=3.3',
     author='William Gomez',
     author_email='william.gomez712@gmail.com',
     url='https://github.com/williamgomez71/RobinApi',
     license='MIT',
     classifiers=[
```

