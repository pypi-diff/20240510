# Comparing `tmp/matroid-1.4.0.tar.gz` & `tmp/matroid-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matroid-1.4.0.tar", last modified: Fri Apr 26 00:41:24 2024, max compression
+gzip compressed data, was "matroid-1.4.1.tar", last modified: Fri May 10 00:12:21 2024, max compression
```

## Comparing `matroid-1.4.0.tar` & `matroid-1.4.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 00:41:24.548307 matroid-1.4.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2024-04-26 00:39:41.000000 matroid-1.4.0/LICENSE.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2024-04-26 00:41:24.548307 matroid-1.4.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8690 2024-04-26 00:39:41.000000 matroid-1.4.0/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 00:41:24.516306 matroid-1.4.0/matroid/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       83 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4259 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1217 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/error.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 00:41:24.528307 matroid-1.4.0/matroid/src/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2193 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/accounts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7816 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/collections.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10796 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/detectors.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9921 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3980 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/images.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5243 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/labels.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      928 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/sse.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10239 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6407 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/temporal_task.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6964 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/video_summary.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3355 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/src/videos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-04-26 00:39:41.000000 matroid-1.4.0/matroid/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 00:41:24.516306 matroid-1.4.0/matroid.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2024-04-26 00:41:24.000000 matroid-1.4.0/matroid.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2024-04-26 00:41:24.000000 matroid-1.4.0/matroid.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-26 00:41:24.000000 matroid-1.4.0/matroid.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-26 00:41:24.000000 matroid-1.4.0/matroid.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2024-04-26 00:41:24.000000 matroid-1.4.0/matroid.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-26 00:41:24.548307 matroid-1.4.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      463 2024-04-26 00:39:41.000000 matroid-1.4.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 00:41:24.548307 matroid-1.4.0/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 00:39:41.000000 matroid-1.4.0/test/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      969 2024-04-26 00:39:41.000000 matroid-1.4.0/test/conftest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      849 2024-04-26 00:39:41.000000 matroid-1.4.0/test/data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2024-04-26 00:39:41.000000 matroid-1.4.0/test/helper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1385 2024-04-26 00:39:41.000000 matroid-1.4.0/test/test_accounts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5714 2024-04-26 00:39:41.000000 matroid-1.4.0/test/test_collections.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11943 2024-04-26 00:39:41.000000 matroid-1.4.0/test/test_detectors_labels.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2328 2024-04-26 00:39:41.000000 matroid-1.4.0/test/test_images.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9925 2024-04-26 00:39:41.000000 matroid-1.4.0/test/test_streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7590 2024-04-26 00:39:41.000000 matroid-1.4.0/test/test_temporal_task.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9491 2024-04-26 00:39:41.000000 matroid-1.4.0/test/test_video_summary.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1385 2024-04-26 00:39:41.000000 matroid-1.4.0/test/test_videos.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-10 00:12:21.385097 matroid-1.4.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2024-05-10 00:10:23.000000 matroid-1.4.1/LICENSE.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2024-05-10 00:12:21.385097 matroid-1.4.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8690 2024-05-10 00:10:23.000000 matroid-1.4.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-10 00:12:21.369097 matroid-1.4.1/matroid/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       83 2024-05-10 00:10:23.000000 matroid-1.4.1/matroid/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2024-05-10 00:10:23.000000 matroid-1.4.1/matroid/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1217 2024-05-10 00:10:23.000000 matroid-1.4.1/matroid/error.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-10 00:12:21.377097 matroid-1.4.1/matroid/src/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-10 00:10:23.000000 matroid-1.4.1/matroid/src/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2193 2024-05-10 00:10:23.000000 matroid-1.4.1/matroid/src/accounts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7816 2024-05-10 00:10:23.000000 matroid-1.4.1/matroid/src/collections.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11132 2024-05-10 00:10:23.000000 matroid-1.4.1/matroid/src/detectors.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9983 2024-05-10 00:10:23.000000 matroid-1.4.1/matroid/src/helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3980 2024-05-10 00:10:23.000000 matroid-1.4.1/matroid/src/images.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5243 2024-05-10 00:10:23.000000 matroid-1.4.1/matroid/src/labels.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      928 2024-05-10 00:10:23.000000 matroid-1.4.1/matroid/src/sse.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10723 2024-05-10 00:10:23.000000 matroid-1.4.1/matroid/src/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6407 2024-05-10 00:10:23.000000 matroid-1.4.1/matroid/src/temporal_task.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6964 2024-05-10 00:10:23.000000 matroid-1.4.1/matroid/src/video_summary.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3355 2024-05-10 00:10:23.000000 matroid-1.4.1/matroid/src/videos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-10 00:10:23.000000 matroid-1.4.1/matroid/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-10 00:12:21.369097 matroid-1.4.1/matroid.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2024-05-10 00:12:21.000000 matroid-1.4.1/matroid.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2024-05-10 00:12:21.000000 matroid-1.4.1/matroid.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-10 00:12:21.000000 matroid-1.4.1/matroid.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-05-10 00:12:21.000000 matroid-1.4.1/matroid.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2024-05-10 00:12:21.000000 matroid-1.4.1/matroid.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-10 00:12:21.385097 matroid-1.4.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      463 2024-05-10 00:10:23.000000 matroid-1.4.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-10 00:12:21.385097 matroid-1.4.1/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-10 00:10:23.000000 matroid-1.4.1/test/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      969 2024-05-10 00:10:23.000000 matroid-1.4.1/test/conftest.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      989 2024-05-10 00:10:23.000000 matroid-1.4.1/test/data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2024-05-10 00:10:23.000000 matroid-1.4.1/test/helper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1385 2024-05-10 00:10:23.000000 matroid-1.4.1/test/test_accounts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5714 2024-05-10 00:10:23.000000 matroid-1.4.1/test/test_collections.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11943 2024-05-10 00:10:23.000000 matroid-1.4.1/test/test_detectors_labels.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2941 2024-05-10 00:10:23.000000 matroid-1.4.1/test/test_images.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10609 2024-05-10 00:10:23.000000 matroid-1.4.1/test/test_streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8440 2024-05-10 00:10:23.000000 matroid-1.4.1/test/test_temporal_task.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9459 2024-05-10 00:10:23.000000 matroid-1.4.1/test/test_video_summary.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1385 2024-05-10 00:10:23.000000 matroid-1.4.1/test/test_videos.py
```

### Comparing `matroid-1.4.0/LICENSE.txt` & `matroid-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `matroid-1.4.0/README.md` & `matroid-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `matroid-1.4.0/matroid/client.py` & `matroid-1.4.1/matroid/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         add_feedback,
         delete_feedback,
     )
     from matroid.src.images import classify_image, localize_image
     from matroid.src.videos import classify_video, get_video_results
     from matroid.src.streams import (
         create_stream,
+        update_stream,
         register_stream,
         delete_monitoring,
         delete_stream,
         watch_monitoring_result,
         get_monitoring_result,
         kill_monitoring,
         monitor_stream,
```

### Comparing `matroid-1.4.0/matroid/error.py` & `matroid-1.4.1/matroid/error.py`

 * *Files identical despite different names*

### Comparing `matroid-1.4.0/matroid/src/accounts.py` & `matroid-1.4.1/matroid/src/accounts.py`

 * *Files identical despite different names*

### Comparing `matroid-1.4.0/matroid/src/collections.py` & `matroid-1.4.1/matroid/src/collections.py`

 * *Files identical despite different names*

### Comparing `matroid-1.4.0/matroid/src/detectors.py` & `matroid-1.4.1/matroid/src/detectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,24 +50,34 @@
         headers = {"Authorization": self.token.authorization_header()}
         data = {"name": name, "detectorType": detectorType}
         data.update(options)
 
         with self.filereader.get_file(file) as file_to_upload:
             # files = {'file': file_to_upload}
             files = {"file": (file, file_to_upload, "application/zip")}
+
+            labels_to_upload = None
+            labelsJSON = data.get("labelsJSON")
+            if labelsJSON:  # Check if labelsJSON is not None or empty
+                with self.filereader.get_file(labelsJSON) as labels_to_upload:
+                    files["labelsJSON"] = labels_to_upload.read()
+                data.pop("labelsJSON")
+
             file_size = os.fstat(file_to_upload.fileno()).st_size
 
             if file_size > MAX_LOCAL_ZIP_SIZE:
                 raise error.InvalidQueryError(
-                    message="File %s is larger than the limit of %d megabytes"
-                    % (file_to_upload.name, self.bytes_to_mb(MAX_LOCAL_ZIP_SIZE))
+                    message=f"File {file_to_upload.name} is larger than the limit of {self.bytes_to_mb(MAX_LOCAL_ZIP_SIZE)} megabytes"
                 )
-            return requests.request(
-                method, endpoint, **{"headers": headers, "files": files, "data": data}
+
+            response = requests.request(
+                method, endpoint, headers=headers, files=files, data=data
             )
+            return response
+
     except Exception as e:
         raise error.APIConnectionError(message=e)
 
 
 # https://staging.app.matroid.com/docs/api/documentation#api-Detectors-DeleteDetectorsDetector_id
 @api_call(error.InvalidQueryError)
 def delete_detector(self, detectorId):
```

### Comparing `matroid-1.4.0/matroid/src/helpers.py` & `matroid-1.4.1/matroid/src/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,14 +191,15 @@
         "classify_image": (base_url + "/detectors/:key/classify_image", "POST"),
         "localize_image": (base_url + "/localize", "POST"),
         # videos
         "classify_video": (base_url + "/detectors/:key/classify_video", "POST"),
         "get_video_results": (base_url + "/videos/:key", "GET"),
         # streams
         "create_stream": (base_url + "/streams", "POST"),
+        "update_stream": (base_url + "/streams/:key", "PUT"),
         "delete_monitoring": (base_url + "/monitorings/:key", "DELETE"),
         "delete_stream": (base_url + "/streams/:key", "DELETE"),
         "watch_monitoring_result": (base_url + "/monitorings/:key/watch", "GET"),
         "get_monitoring_result": (base_url + "/monitorings/:key", "GET"),
         "kill_monitoring": (base_url + "/monitorings/:key/kill", "POST"),
         "monitor_stream": (base_url + "/streams/:streamId/monitor/:detectorId", "POST"),
         "update_monitoring": (base_url + "/monitorings/:monitoringId", "PUT"),
```

### Comparing `matroid-1.4.0/matroid/src/images.py` & `matroid-1.4.1/matroid/src/images.py`

 * *Files identical despite different names*

### Comparing `matroid-1.4.0/matroid/src/labels.py` & `matroid-1.4.1/matroid/src/labels.py`

 * *Files identical despite different names*

### Comparing `matroid-1.4.0/matroid/src/sse.py` & `matroid-1.4.1/matroid/src/sse.py`

 * *Files identical despite different names*

### Comparing `matroid-1.4.0/matroid/src/streams.py` & `matroid-1.4.1/matroid/src/streams.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,29 @@
         raise error.APIConnectionError(message=e)
 
 
 # register_stream is now DEPRECATED in favor of create_stream (kept for backwards-compatibility)
 register_stream = create_stream
 
 
+@api_call(error.InvalidQueryError)
+def update_stream(self, streamId, **options):
+    (endpoint, method) = self.endpoints["update_stream"]
+    endpoint = endpoint.replace(":key", streamId)
+
+    try:
+        headers = {"Authorization": self.token.authorization_header()}
+        data = {}
+        data.update(options)
+
+        return requests.request(method, endpoint, **{"headers": headers, "json": data})
+    except Exception as e:
+        raise error.APIConnectionError(message=e)
+
+
 # https://staging.app.matroid.com/docs/api/documentation#api-Streams-DeleteMonitoringsMonitoring_id
 @api_call(error.InvalidQueryError)
 def delete_monitoring(self, monitoringId):
     (endpoint, method) = self.endpoints["delete_monitoring"]
     endpoint = endpoint.replace(":key", monitoringId)
 
     try:
```

### Comparing `matroid-1.4.0/matroid/src/temporal_task.py` & `matroid-1.4.1/matroid/src/temporal_task.py`

 * *Files identical despite different names*

### Comparing `matroid-1.4.0/matroid/src/video_summary.py` & `matroid-1.4.1/matroid/src/video_summary.py`

 * *Files identical despite different names*

### Comparing `matroid-1.4.0/matroid/src/videos.py` & `matroid-1.4.1/matroid/src/videos.py`

 * *Files identical despite different names*

### Comparing `matroid-1.4.0/matroid.egg-info/SOURCES.txt` & `matroid-1.4.1/matroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matroid-1.4.0/test/conftest.py` & `matroid-1.4.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `matroid-1.4.0/test/data.py` & `matroid-1.4.1/test/data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import os
 
 EVERYDAY_OBJECT_DETECTOR_ID = "598e23679fd1a805a5c09275"
+EVERYDAY_OBJECT_SEGMENTOR_ID = "62bb48b7b80c90542d4e8a55"
+TAL_DETECTOR_ID = "662fdc71c8630f813831c024"
+TAL_DETECTOR_LABELS = ["Full Cycle"]
 DETECTOR_LABELS = ["person", "boat"]
 DEFAULT_DETECTION_THRESHOLD = 0.5
 RANDOM_MONGO_ID = "5d0148512563ae5e748e9a66"
 
 TEST_IMAGE_URL = (
     "https://m-test-public.s3.amazonaws.com/test/python-client/tesla-cat.jpg"
 )
```

### Comparing `matroid-1.4.0/test/test_accounts.py` & `matroid-1.4.1/test/test_accounts.py`

 * *Files identical despite different names*

### Comparing `matroid-1.4.0/test/test_collections.py` & `matroid-1.4.1/test/test_collections.py`

 * *Files identical despite different names*

### Comparing `matroid-1.4.0/test/test_detectors_labels.py` & `matroid-1.4.1/test/test_detectors_labels.py`

 * *Files identical despite different names*

### Comparing `matroid-1.4.0/test/test_images.py` & `matroid-1.4.1/test/test_images.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from test.data import (
     TEST_IMAGE_URL,
     TEST_IMAGE_URL_DOG,
     TEST_IMAGE_FILE,
     TEST_IMAGE_FILE_DOG,
     EVERYDAY_OBJECT_DETECTOR_ID,
+    EVERYDAY_OBJECT_SEGMENTOR_ID,
 )
 from matroid.error import InvalidQueryError, APIError
 from test.helper import print_test_pass
 
 
 class TestImages(object):
     def test_images(self, set_up_client):
@@ -25,14 +26,20 @@
         #     detector_id=EVERYDAY_OBJECT_DETECTOR_ID, url=TEST_IMAGE_URL, file=TEST_IMAGE_FILE, urls=urls, files=files)
         self.localize_image_test(
             localizer=EVERYDAY_OBJECT_DETECTOR_ID,
             localizer_label=localizer_label,
             url=TEST_IMAGE_URL,
         )
 
+        self.segment_image_test(
+            detector_id=EVERYDAY_OBJECT_SEGMENTOR_ID,
+            url=TEST_IMAGE_URL,
+            expected_label=localizer_label,
+        )
+
     def classify_image_test(self, detector_id, url, urls, file, files):
         with pytest.raises(APIError) as e:
             # self.api.classify_image(detectorId=detector_id, url='invalid-url')
             self.api.classify_image(detectorId=detector_id)
         assert "invalid_query_err" in str(e)
         print("Classify invalid url test passed")
 
@@ -59,7 +66,16 @@
     def localize_image_test(self, localizer, localizer_label, url):
         res = self.api.localize_image(
             localizer=localizer, localizerLabel=localizer_label, url=url
         )
         assert res["results"][0]["predictions"] != None
 
         print_test_pass()
+
+    def segment_image_test(self, detector_id, url, expected_label):
+        res = self.api.classify_image(detectorId=detector_id, url=url)
+        preds = res["results"][0]["predictions"]
+        assert len(preds) == 3, "Expected 3 predictions for Segmentation"
+        assert expected_label in preds[0]["labels"]
+        assert len(preds[0]["segments"][0]["extPoints"]) > 500
+
+        print_test_pass()
```

### Comparing `matroid-1.4.0/test/test_streams.py` & `matroid-1.4.1/test/test_streams.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,20 @@
         minDetectionInterval = 90
         # set up client
         self.api = set_up_client
 
         # start testing
         try:
             stream_id = self.create_stream_test(url=TEST_S3_VIDEO_URL, name=stream_name)
+            self.update_stream_test(
+                stream_id,
+                "new-name",
+                "5",
+                [{"key": "i am a key", "template": "and i am a template"}],
+            )
             stream_id_2 = self.register_stream_test(
                 url=TEST_S3_VIDEO_URL_2, name=stream_name_2
             )
             monitoring_id = self.monitor_stream_test(
                 stream_id=stream_id,
                 detector_id=EVERYDAY_OBJECT_DETECTOR_ID,
                 thresholds=thresholds,
@@ -89,14 +95,28 @@
         with pytest.raises(APIError) as e:
             self.api.create_stream(url=url, name=name)
         assert "invalid_query_err" in str(e)
 
         print_test_pass()
         return res["streamId"]
 
+    def update_stream_test(self, stream_id, name, retention_days, custom_fields):
+        res = self.api.update_stream(
+            streamId=stream_id,
+            name=name,
+            retentionDays=retention_days,
+            customFields=custom_fields,
+        )
+        assert res["feed"] == stream_id
+        assert res["name"] == name
+        assert str(res["retentionDays"]) == retention_days
+        assert res["customFields"] == custom_fields
+
+        print_test_pass()
+
     def register_stream_test(self, url, name):
         res = self.api.register_stream(url=url, name=name)
         assert res["streamId"] != None
 
         with pytest.raises(APIError) as e:
             self.api.register_stream(url=url, name=name)
         assert "invalid_query_err" in str(e)
```

### Comparing `matroid-1.4.0/test/test_temporal_task.py` & `matroid-1.4.1/test/test_temporal_task.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 import random
 
 from test.data import (
     TEST_LOCAL_VIDEO_URL,
     TEST_S3_VIDEO_URL,
     TEST_VIDEO_URL,
     EVERYDAY_OBJECT_DETECTOR_ID,
+    TAL_DETECTOR_ID,
     DETECTOR_LABELS,
+    TAL_DETECTOR_LABELS,
     DEFAULT_DETECTION_THRESHOLD,
 )
 from matroid.error import APIError
 from test.helper import print_test_pass
 
 
 class TestTemporalTask(object):
@@ -69,44 +71,52 @@
         url=None,
         videoId=None,
         file=None,
     ):
         if url and file:
             with pytest.raises(APIError) as e:
                 self.api.localize_video_actions(
-                    detectorId=EVERYDAY_OBJECT_DETECTOR_ID,
+                    detectorId=TAL_DETECTOR_ID,
                     url=url,
                     file=file,
-                    labels=DETECTOR_LABELS,
+                    labels=TAL_DETECTOR_LABELS,
                 )
             assert "You may only specify a file or a URL, not both" in str(e)
 
         if url:
             with pytest.raises(APIError) as e:
                 self.api.localize_video_actions(
+                    detectorId=TAL_DETECTOR_ID,
+                    url=TEST_LOCAL_VIDEO_URL,
+                    labels=TAL_DETECTOR_LABELS,
+                )
+            assert "You provided an invalid URL" in str(e)
+
+            with pytest.raises(APIError) as e:
+                self.api.localize_video_actions(
                     detectorId=EVERYDAY_OBJECT_DETECTOR_ID,
                     url=TEST_LOCAL_VIDEO_URL,
                     labels=DETECTOR_LABELS,
                 )
-            assert "You provided an invalid URL" in str(e)
+            assert "This detector does not support TAL" in str(e)
 
             res = self.api.localize_video_actions(
-                detectorId=EVERYDAY_OBJECT_DETECTOR_ID,
+                detectorId=TAL_DETECTOR_ID,
                 url=url,
-                labels=DETECTOR_LABELS,
+                labels=TAL_DETECTOR_LABELS,
             )
 
         if file:
             res = self.api.localize_video_actions(
-                detectorId=EVERYDAY_OBJECT_DETECTOR_ID,
+                detectorId=TAL_DETECTOR_ID,
                 file=file,
-                labels=DETECTOR_LABELS,
+                labels=TAL_DETECTOR_LABELS,
             )
 
-        assert res["temporal_task"]["network"] == EVERYDAY_OBJECT_DETECTOR_ID
+        assert res["temporal_task"]["network"] == TAL_DETECTOR_ID
 
         print_test_pass()
         return res["temporal_task"]["_id"]
 
     def get_temporal_task_test(self, taskId):
         with pytest.raises(APIError) as e:
             self.api.get_temporal_task(taskId="123")
@@ -163,52 +173,65 @@
 
     def create_stream_temporal_task_test(self, streamId, startTime, endTime):
         with pytest.raises(APIError) as e:
             self.api.localize_stream_actions(
                 streamId=streamId,
                 startTime="test",
                 endTime=endTime,
-                detectorId=EVERYDAY_OBJECT_DETECTOR_ID,
-                labels=DETECTOR_LABELS,
-                thresholds=[DEFAULT_DETECTION_THRESHOLD] * len(DETECTOR_LABELS),
+                detectorId=TAL_DETECTOR_ID,
+                labels=TAL_DETECTOR_LABELS,
+                thresholds=[DEFAULT_DETECTION_THRESHOLD] * len(TAL_DETECTOR_LABELS),
             )
         assert "Invalid dates provided" in str(e)
         with pytest.raises(APIError) as e:
             self.api.localize_stream_actions(
+                detectorId=TAL_DETECTOR_ID,
+                labels=TAL_DETECTOR_LABELS,
+                streamId=streamId,
+                startTime=datetime.utcfromtimestamp(
+                    int(time.time()) - (24 * 60 * 60 * 8)
+                ),
+                endTime=endTime,
+                thresholds=[DEFAULT_DETECTION_THRESHOLD] * len(TAL_DETECTOR_LABELS),
+            )
+        assert "Provided dates are not within your stream" in str(e)
+
+        with pytest.raises(APIError) as e:
+            self.api.localize_stream_actions(
                 detectorId=EVERYDAY_OBJECT_DETECTOR_ID,
                 labels=DETECTOR_LABELS,
                 streamId=streamId,
                 startTime=datetime.utcfromtimestamp(
                     int(time.time()) - (24 * 60 * 60 * 8)
                 ),
                 endTime=endTime,
                 thresholds=[DEFAULT_DETECTION_THRESHOLD] * len(DETECTOR_LABELS),
             )
-        assert "Provided dates are not within your stream" in str(e)
+        assert "This detector does not support TAL" in str(e)
 
         res = self.api.localize_stream_actions(
             streamId,
             startTime,
             endTime,
-            detectorId=EVERYDAY_OBJECT_DETECTOR_ID,
-            labels=DETECTOR_LABELS,
-            thresholds=[DEFAULT_DETECTION_THRESHOLD] * len(DETECTOR_LABELS),
+            detectorId=TAL_DETECTOR_ID,
+            labels=TAL_DETECTOR_LABELS,
+            thresholds=[DEFAULT_DETECTION_THRESHOLD] * len(TAL_DETECTOR_LABELS),
         )
         assert res["temporal_task"]["feed"] == streamId
         assert (
             datetime.strptime(
                 res["temporal_task"]["startTime"], "%Y-%m-%dT%H:%M:%S.000Z"
             )
             == startTime
         )
         assert (
             datetime.strptime(res["temporal_task"]["endTime"], "%Y-%m-%dT%H:%M:%S.000Z")
             == endTime
         )
-        assert res["temporal_task"]["network"] == EVERYDAY_OBJECT_DETECTOR_ID
+        assert res["temporal_task"]["network"] == TAL_DETECTOR_ID
 
         print_test_pass()
         return res["temporal_task"]["_id"]
 
     def get_stream_temporal_tasks_test(self, streamId):
         res = self.api.get_stream_temporal_tasks(streamId)
         assert len(res["temporal_tasks"]) == 1
```

### Comparing `matroid-1.4.0/test/test_video_summary.py` & `matroid-1.4.1/test/test_video_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
         print_test_pass()
         return res["summary"]["_id"]
 
     def get_video_summary_test(self, summaryId):
         with pytest.raises(APIError) as e:
             self.api.get_video_summary(summaryId="123")
-        assert "invalid_query_err" in str(e)
+        assert "Forbidden" in str(e)
 
         res = self.api.get_video_summary(summaryId=summaryId)
 
         assert res["progress"] >= 0 and res["progress"] <= 1
         assert res["state"] in [
             "requested",
             "preparing",
@@ -124,22 +124,22 @@
         ]
 
         print_test_pass()
 
     def get_video_summary_tracks_test(self):
         with pytest.raises(APIError) as e:
             self.api.get_video_summary_tracks(summaryId="123")
-        assert "invalid_query_err" in str(e)
+        assert "Forbidden" in str(e)
 
         print_test_pass()
 
     def get_video_summary_file_test(self):
         with pytest.raises(APIError) as e:
             self.api.get_video_summary_file(summaryId="123")
-        assert "invalid_query_err" in str(e)
+        assert "Forbidden" in str(e)
 
         print_test_pass()
 
     def create_stream_summary_test(self, streamId, startTime, endTime):
         with pytest.raises(APIError) as e:
             self.api.create_stream_summary(
                 streamId=streamId,
@@ -203,15 +203,15 @@
         res = self.api.delete_stream(streamId=streamId)
         assert res["message"] == "Successfully deleted stream."
         print_test_pass()
 
     def delete_video_summary_test(self, summaryId):
         with pytest.raises(APIError) as e:
             self.api.delete_video_summary(summaryId="123")
-        assert "invalid_query_err" in str(e)
+        assert "Forbidden" in str(e)
 
         res = self.api.delete_video_summary(summaryId=summaryId)
         assert res["summaryId"] == summaryId
         print_test_pass()
 
     def get_existing_summaries_test(self, *summary_ids):
         res = self.api.get_existing_summaries()
```

### Comparing `matroid-1.4.0/test/test_videos.py` & `matroid-1.4.1/test/test_videos.py`

 * *Files identical despite different names*

