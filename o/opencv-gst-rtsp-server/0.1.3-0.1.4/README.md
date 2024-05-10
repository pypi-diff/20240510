# Comparing `tmp/opencv_gst_rtsp_server-0.1.3.tar.gz` & `tmp/opencv_gst_rtsp_server-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencv_gst_rtsp_server-0.1.3.tar", last modified: Fri Jul 28 08:55:24 2023, max compression
+gzip compressed data, was "opencv_gst_rtsp_server-0.1.4.tar", last modified: Fri May 10 07:55:30 2024, max compression
```

## Comparing `opencv_gst_rtsp_server-0.1.3.tar` & `opencv_gst_rtsp_server-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:55:24.311378 opencv_gst_rtsp_server-0.1.3/
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     1975 2023-07-28 08:55:24.311378 opencv_gst_rtsp_server-0.1.3/PKG-INFO
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      880 2023-07-28 08:55:16.000000 opencv_gst_rtsp_server-0.1.3/README.md
-drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:55:24.307378 opencv_gst_rtsp_server-0.1.3/build/
-drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:55:24.311378 opencv_gst_rtsp_server-0.1.3/build/opencv_gst_rtsp_server.egg-info/
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      787 2023-07-28 08:55:24.000000 opencv_gst_rtsp_server-0.1.3/build/opencv_gst_rtsp_server.egg-info/SOURCES.txt
-drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:55:24.311378 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      458 2023-07-28 08:55:16.000000 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/__init__.py
-drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:55:24.311378 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/exception/
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 04:16:13.000000 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/exception/__init__.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      200 2023-07-28 04:12:31.000000 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/exception/network_exception.py
-drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:55:24.311378 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/rtsp_media_factory/
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 04:16:16.000000 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/rtsp_media_factory/__init__.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     1727 2023-07-28 04:13:53.000000 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/rtsp_media_factory/opencv_frame_media_factory.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     1522 2023-07-28 04:13:59.000000 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/rtsp_media_factory/opencv_media_factory.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     2315 2023-07-28 04:14:05.000000 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/rtsp_media_factory/opencv_stream_media_factory.py
-drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:55:24.311378 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/rtsp_server/
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 04:16:18.000000 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/rtsp_server/__init__.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      616 2023-07-28 04:14:10.000000 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/rtsp_server/opencv_frame_rtsp_server.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     2302 2023-07-28 04:14:18.000000 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/rtsp_server/opencv_rtsp_server.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      515 2023-07-28 04:14:22.000000 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/rtsp_server/opencv_stream_rtsp_server.py
-drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:55:24.311378 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/utils/
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 04:16:21.000000 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/utils/__init__.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      334 2023-07-28 04:12:44.000000 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/utils/log_utils.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      621 2023-07-28 04:12:44.000000 opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/utils/network_utils.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      151 2023-07-28 08:55:24.311378 opencv_gst_rtsp_server-0.1.3/setup.cfg
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     1118 2023-07-28 08:55:16.000000 opencv_gst_rtsp_server-0.1.3/setup.py
+drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2024-05-10 07:55:30.783118 opencv_gst_rtsp_server-0.1.4/
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     1975 2024-05-10 07:55:30.783118 opencv_gst_rtsp_server-0.1.4/PKG-INFO
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      880 2023-07-28 08:55:16.000000 opencv_gst_rtsp_server-0.1.4/README.md
+drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2024-05-10 07:55:30.783118 opencv_gst_rtsp_server-0.1.4/build/
+drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2024-05-10 07:55:30.783118 opencv_gst_rtsp_server-0.1.4/build/opencv_gst_rtsp_server.egg-info/
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      886 2024-05-10 07:55:30.000000 opencv_gst_rtsp_server-0.1.4/build/opencv_gst_rtsp_server.egg-info/SOURCES.txt
+drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2024-05-10 07:55:30.783118 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      392 2024-05-10 07:35:46.000000 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/__init__.py
+drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2024-05-10 07:55:30.783118 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/exception/
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 04:16:13.000000 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/exception/__init__.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      229 2023-09-27 18:01:26.000000 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/exception/element_exception.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      200 2023-07-28 04:12:31.000000 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/exception/network_exception.py
+drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2024-05-10 07:55:30.783118 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/rtsp_media_factory/
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 04:16:16.000000 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/rtsp_media_factory/__init__.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     1862 2024-05-10 07:35:46.000000 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/rtsp_media_factory/opencv_frame_media_factory.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     3340 2024-05-10 07:35:46.000000 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/rtsp_media_factory/opencv_media_factory.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     2449 2024-05-10 07:35:46.000000 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/rtsp_media_factory/opencv_stream_media_factory.py
+drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2024-05-10 07:55:30.783118 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/rtsp_server/
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 04:16:18.000000 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/rtsp_server/__init__.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      680 2024-05-10 07:35:46.000000 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/rtsp_server/opencv_frame_rtsp_server.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     2652 2024-05-10 07:35:46.000000 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/rtsp_server/opencv_rtsp_server.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      543 2024-05-10 07:35:46.000000 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/rtsp_server/opencv_stream_rtsp_server.py
+drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2024-05-10 07:55:30.783118 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/utils/
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 04:16:21.000000 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/utils/__init__.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      485 2023-09-27 18:01:53.000000 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/utils/gst_utils.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      621 2023-07-28 04:12:44.000000 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/utils/network_utils.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     1111 2023-08-21 04:01:40.000000 opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/utils/thread_utils.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      151 2024-05-10 07:55:30.787119 opencv_gst_rtsp_server-0.1.4/setup.cfg
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     1119 2024-05-10 07:54:59.000000 opencv_gst_rtsp_server-0.1.4/setup.py
```

### Comparing `opencv_gst_rtsp_server-0.1.3/PKG-INFO` & `opencv_gst_rtsp_server-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencv_gst_rtsp_server
-Version: 0.1.3
+Version: 0.1.4
 Summary: Restream rtsp with opencv frame using gst-rtsp-server
 Home-page: https://github.com/nguyencobap/opencv_gst_rtsp_server
 Author: Nguyen Hai Nguyen
 Author-email: nguyenhainguyen97@gmail.com
 License: MIT License
 Description: ## What is this?
```

### Comparing `opencv_gst_rtsp_server-0.1.3/README.md` & `opencv_gst_rtsp_server-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `opencv_gst_rtsp_server-0.1.3/build/opencv_gst_rtsp_server.egg-info/SOURCES.txt` & `opencv_gst_rtsp_server-0.1.4/build/opencv_gst_rtsp_server.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 README.md
 setup.cfg
 setup.py
 opencv_gst_rtsp_server/__init__.py
 opencv_gst_rtsp_server/exception/__init__.py
+opencv_gst_rtsp_server/exception/element_exception.py
 opencv_gst_rtsp_server/exception/network_exception.py
 opencv_gst_rtsp_server/rtsp_media_factory/__init__.py
 opencv_gst_rtsp_server/rtsp_media_factory/opencv_frame_media_factory.py
 opencv_gst_rtsp_server/rtsp_media_factory/opencv_media_factory.py
 opencv_gst_rtsp_server/rtsp_media_factory/opencv_stream_media_factory.py
 opencv_gst_rtsp_server/rtsp_server/__init__.py
 opencv_gst_rtsp_server/rtsp_server/opencv_frame_rtsp_server.py
 opencv_gst_rtsp_server/rtsp_server/opencv_rtsp_server.py
 opencv_gst_rtsp_server/rtsp_server/opencv_stream_rtsp_server.py
 opencv_gst_rtsp_server/utils/__init__.py
-opencv_gst_rtsp_server/utils/log_utils.py
-opencv_gst_rtsp_server/utils/network_utils.py
+opencv_gst_rtsp_server/utils/gst_utils.py
+opencv_gst_rtsp_server/utils/network_utils.py
+opencv_gst_rtsp_server/utils/thread_utils.py
```

### Comparing `opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/rtsp_media_factory/opencv_frame_media_factory.py` & `opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/rtsp_media_factory/opencv_frame_media_factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,42 @@
-from opencv_gst_rtsp_server.utils.log_utils import logger
-from opencv_gst_rtsp_server.rtsp_media_factory.opencv_media_factory import OpenCVMediaFactory
 import gi
+
+from .opencv_media_factory  import OpenCVMediaFactory
+
 gi.require_version('Gst', '1.0')
 from gi.repository import Gst
 
+import logging
+logger = logging.getLogger(__name__)
+
 class OpenCVFrameMediaFactory(OpenCVMediaFactory):
-    def __init__(self, width: int, height: int, fps: int, **properties):
+    def __init__(self, width: int, height: int, fps: int, channel: int = 3, use_gpu: bool = False, use_h265: bool = False, **properties):
         super(OpenCVFrameMediaFactory, self).__init__(**properties)
-        self.number_frames = 0
         self.width = width
         self.height = height
+        self.channel = channel
         self.fps = fps
+        self.use_gpu = use_gpu
+        self.use_h265 = use_h265
         self.frame = None
         self.duration = 1 / self.fps * Gst.SECOND  # duration of a frame in nanoseconds
-        logger.debug(f"self.width = {self.width}, self.height = {self.height}, self.fps = {self.fps}, self.duration = {self.duration}")
+        logger.debug(f"self.width = {self.width}, self.height = {self.height}, self.channel = {self.channel}, self.fps = {self.fps}, self.duration = {self.duration}")
 
     def set_frame(self, frame):
         self.frame = frame
 
     def on_need_data(self, src, length: int):
         if self.frame is not None:
             data = self.frame.tostring()
             buf = Gst.Buffer.new_allocate(None, len(data), None)
             buf.fill(0, data)
             buf.duration = self.duration
-            timestamp = self.number_frames * self.duration
+            timestamp = self.frame_num_dict[src] * self.duration
             buf.pts = buf.dts = int(timestamp)
             buf.offset = timestamp
-            self.number_frames += 1
+            self.frame_num_dict[src] += 1
             retval = src.emit('push-buffer', buf)
-            logger.debug('pushed buffer, frame {}, duration {} ns, durations {} s'.format(self.number_frames,
+            logger.debug('pushed buffer, frame {}, duration {} ns, durations {} s'.format(self.frame_num_dict[src],
                                                                                     self.duration,
                                                                                     self.duration / Gst.SECOND))
             if retval != Gst.FlowReturn.OK:
                 logger.debug(retval)
```

### Comparing `opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/rtsp_media_factory/opencv_stream_media_factory.py` & `opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/rtsp_media_factory/opencv_stream_media_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,57 @@
 import cv2
 import gi
 
 gi.require_version('Gst', '1.0')
 gi.require_version('GstRtspServer', '1.0')
-from gi.repository import Gst, GstRtspServer, GstRtsp
-from opencv_gst_rtsp_server.utils.log_utils import logger
-from opencv_gst_rtsp_server.rtsp_media_factory.opencv_media_factory import OpenCVMediaFactory
+from gi.repository import Gst, GstRtsp, GstRtspServer
+
+from .opencv_media_factory import OpenCVMediaFactory
+
+import logging
+logger = logging.getLogger(__name__)
+
 
 class OpenCVStreamMediaFactory(OpenCVMediaFactory):
-    def __init__(self, stream_link: str, **properties):
+    def __init__(self, stream_link: str, channel: int = 3, use_gpu: bool = False, use_h265: bool = False, **properties):
         super(OpenCVStreamMediaFactory, self).__init__(**properties)
         if stream_link.isnumeric():
             self.stream_link = int(stream_link)
         else:
             self.stream_link = stream_link
-
+        self.use_gpu = use_gpu
+        self.use_h265 = use_h265
         self.cap = cv2.VideoCapture(self.stream_link)
 
-        self.number_frames = 0
         self.width = int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
         self.width = self.width if self.width > 0 else 1920
 
         self.height = int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
         self.height = self.height if self.height > 0 else 1080
+
+        self.channel = channel
         
         self.fps = int(self.cap.get(cv2.CAP_PROP_FPS))
         self.fps = self.fps if  60 > self.fps > 0 else 30
 
         self.duration = 1 / self.fps * Gst.SECOND  # duration of a frame in nanoseconds
-        logger.debug(f"self.width = {self.width}, self.height = {self.height}, self.fps = {self.fps}, self.duration = {self.duration}")
+        logger.debug(f"self.width = {self.width}, self.height = {self.height}, self.channel = {self.channel}, self.fps = {self.fps}, self.duration = {self.duration}")
 
      
     def on_need_data(self, src, length: int):
         if self.cap.isOpened():
             ret, frame = self.cap.read()
             if ret:
                 data = frame.tostring()
                 buf = Gst.Buffer.new_allocate(None, len(data), None)
                 buf.fill(0, data)
                 buf.duration = self.duration
-                timestamp = self.number_frames * self.duration
+                timestamp = self.frame_num_dict[src] * self.duration
                 buf.pts = buf.dts = int(timestamp)
                 buf.offset = timestamp
-                self.number_frames += 1
+                self.frame_num_dict[src] += 1
                 retval = src.emit('push-buffer', buf)
-                logger.debug('pushed buffer, frame {}, duration {} ns, durations {} s'.format(self.number_frames,
+                logger.debug('pushed buffer, frame {}, duration {} ns, durations {} s'.format(self.frame_num_dict[src],
                                                                                        self.duration,
                                                                                        self.duration / Gst.SECOND))
                 if retval != Gst.FlowReturn.OK:
                     logger.debug(retval)
```

### Comparing `opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/rtsp_server/opencv_frame_rtsp_server.py` & `opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/rtsp_server/opencv_frame_rtsp_server.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
-from opencv_gst_rtsp_server.rtsp_media_factory.opencv_frame_media_factory import OpenCVFrameMediaFactory
-from opencv_gst_rtsp_server.rtsp_server.opencv_rtsp_server import OpenCVRTSPServer
+from ..rtsp_media_factory.opencv_frame_media_factory import OpenCVFrameMediaFactory
+from .opencv_rtsp_server import OpenCVRTSPServer
+
 
 class OpenCVFrameRTSPServer(OpenCVRTSPServer):
-    def __init__(self, width: int, height: int, fps: int, port: int, endpoint: str = "/stream", **properties):
-        factory = OpenCVFrameMediaFactory(width=width, height=height, fps=fps)
+    def __init__(self, width: int, height: int, fps: int, port: int, channel: int = 3, endpoint: str = "/stream", use_gpu: bool = False, use_h265: bool = False, **properties):
+        factory = OpenCVFrameMediaFactory(width=width, height=height, channel=channel, fps=fps, use_gpu=use_gpu, use_h265=use_h265)
         super(OpenCVFrameRTSPServer, self).__init__(factory=factory, endpoint=endpoint, port=port, **properties)
 
     def set_frame(self, frame):
         self.factory.set_frame(frame=frame)
```

### Comparing `opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/rtsp_server/opencv_rtsp_server.py` & `opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/rtsp_server/opencv_rtsp_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import gi
 
 gi.require_version('Gst', '1.0')
 gi.require_version('GstRtspServer', '1.0')
 from gi.repository import Gst, GstRtspServer, GObject
-from opencv_gst_rtsp_server.utils.network_utils import NetworkUtils
-from opencv_gst_rtsp_server.rtsp_media_factory.opencv_media_factory import OpenCVMediaFactory
-from opencv_gst_rtsp_server.exception.network_exception import PortAlreadyInUseException
+from ..utils.network_utils import NetworkUtils
+from ..rtsp_media_factory.opencv_media_factory import OpenCVMediaFactory
+from ..exception.network_exception import PortAlreadyInUseException
 from threading import Thread
-from opencv_gst_rtsp_server.utils.log_utils import logger
+from ..utils.thread_utils import ThreadUtilities
+
+import logging
+logger = logging.getLogger(__name__)
 
 class OpenCVRTSPServer(GstRtspServer.RTSPServer):
     thread: Thread = None
     main_loop: GObject.MainLoop = None
+    server_id: int
     factory: OpenCVMediaFactory = None
     endpoint: str = "/stream"
     port: int
 
     def __init__(self, factory: OpenCVMediaFactory, port: int, endpoint: str = "/stream", **properties):
         super(OpenCVRTSPServer, self).__init__(**properties)
         self.endpoint = endpoint
@@ -24,28 +28,28 @@
 
         if NetworkUtils.is_port_in_use(port=self.port):
             raise PortAlreadyInUseException(port=self.port)
         self.set_service(str(self.port))
 
         self.factory.set_shared(True)
         self.get_mount_points().add_factory(self.endpoint, self.factory)
-        self.attach(None)
 
     def get_port(self) -> int:
         return self.port
     
     def get_endpoint(self) -> str:
         return self.endpoint
 
     def start(self):
         if self.main_loop is None or not self.main_loop.is_running():
             GObject.threads_init()
             Gst.init(None)
 
             self.main_loop = GObject.MainLoop()
+            self.server_id = self.attach(self.main_loop.get_context())
             self.main_loop.run()
         else:
             logger.debug("Main loop has already been run")
 
     def start_background(self) -> Thread:
         if self.thread is None or not self.thread.is_alive():
             self.thread = Thread(target=self.start)
@@ -60,8 +64,18 @@
             self.factory.stop()
         else:
             logger.debug("Factory is None")
 
         if self.main_loop and self.main_loop.is_running():
             self.main_loop.quit()
         else:
-            logger.debug("Main loop has already been quit")
+            logger.debug("Main loop has already been quit")
+        
+        GObject.source_remove(self.server_id)
+
+        if self.thread:
+            try:
+                ThreadUtilities.async_raise(self.thread.ident)
+            except:
+                logger.error("Stop thread failed", exc_info=True)
+        else:
+            logger.debug("self.thread null")
```

### Comparing `opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/rtsp_server/opencv_stream_rtsp_server.py` & `opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/rtsp_server/opencv_stream_rtsp_server.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 
-from opencv_gst_rtsp_server.rtsp_media_factory.opencv_stream_media_factory import OpenCVStreamMediaFactory
-from opencv_gst_rtsp_server.rtsp_server.opencv_rtsp_server import OpenCVRTSPServer
+from ..rtsp_media_factory.opencv_stream_media_factory import OpenCVStreamMediaFactory
+from .opencv_rtsp_server import OpenCVRTSPServer
 
 class OpenCVStreamRTSPServer(OpenCVRTSPServer):
-    def __init__(self, stream_link: str, port: int, endpoint: str = "/stream", **properties):
-        factory = OpenCVStreamMediaFactory(stream_link=stream_link)
+    def __init__(self, stream_link: str, port: int, endpoint: str = "/stream", use_gpu: bool = False, use_h265: bool = False, **properties):
+        factory = OpenCVStreamMediaFactory(stream_link=stream_link, use_gpu=use_gpu, use_h265=use_h265)
         super(OpenCVStreamRTSPServer, self).__init__(factory=factory, endpoint=endpoint, port=port, **properties)
```

### Comparing `opencv_gst_rtsp_server-0.1.3/opencv_gst_rtsp_server/utils/network_utils.py` & `opencv_gst_rtsp_server-0.1.4/opencv_gst_rtsp_server/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `opencv_gst_rtsp_server-0.1.3/setup.py` & `opencv_gst_rtsp_server-0.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import io
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 long_description = io.open("README.md", encoding="utf-8").read()
 
 setup(
     name='opencv_gst_rtsp_server',
-    version='0.1.3',    
+    version='0.1.4',    
     description='Restream rtsp with opencv frame using gst-rtsp-server',
     url='https://github.com/nguyencobap/opencv_gst_rtsp_server',
     author='Nguyen Hai Nguyen',
     author_email='nguyenhainguyen97@gmail.com',
     license='MIT License',
     python_requires=">=3.5",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['gstreamer', 'gst', 'opencv', 'rtsp'],
     install_requires=['opencv-python>=4.6.0.66',
-                        'pycairo>=1.24.0',
-                        'PyGObject>=3.44.1'
+                        'pycairo>=1.20.1',
+                        'PyGObject>=3.42.2'
                         ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Multimedia :: Video',
         'License :: OSI Approved :: MIT License',  
         'Operating System :: POSIX :: Linux',
```

