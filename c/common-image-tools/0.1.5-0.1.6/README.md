# Comparing `tmp/common_image_tools-0.1.5.tar.gz` & `tmp/common_image_tools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_image_tools-0.1.5.tar", max compression
+gzip compressed data, was "common_image_tools-0.1.6.tar", max compression
```

## Comparing `common_image_tools-0.1.5.tar` & `common_image_tools-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-05-06 18:16:59.565000 common_image_tools-0.1.5/common_image_tools/__init__.py
--rw-r--r--   0        0        0     2768 2024-04-26 23:47:44.007193 common_image_tools-0.1.5/common_image_tools/conversion.py
--rw-r--r--   0        0        0     2180 2024-04-26 23:47:44.020791 common_image_tools-0.1.5/common_image_tools/operation.py
--rw-r--r--   0        0        0     5816 2024-04-26 23:47:44.043038 common_image_tools-0.1.5/common_image_tools/tool.py
--rw-r--r--   0        0        0     1359 2024-04-26 23:47:44.057023 common_image_tools-0.1.5/common_image_tools/verification.py
--rw-r--r--   0        0        0      266 2024-04-26 23:47:44.073210 common_image_tools-0.1.5/common_image_tools/visualization.py
--rw-r--r--   0        0        0      607 2024-04-26 23:47:44.088914 common_image_tools-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      832 2024-04-26 23:47:44.005195 common_image_tools-0.1.5/README.md
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 common_image_tools-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 18:16:59.565000 common_image_tools-0.1.6/common_image_tools/__init__.py
+-rw-r--r--   0        0        0     2794 2024-05-10 11:40:01.955405 common_image_tools-0.1.6/common_image_tools/conversion.py
+-rw-r--r--   0        0        0     2211 2024-05-10 11:41:04.437528 common_image_tools-0.1.6/common_image_tools/operation.py
+-rw-r--r--   0        0        0     5867 2024-05-10 11:42:17.895318 common_image_tools-0.1.6/common_image_tools/tool.py
+-rw-r--r--   0        0        0     1359 2024-04-26 23:47:44.057023 common_image_tools-0.1.6/common_image_tools/verification.py
+-rw-r--r--   0        0        0      266 2024-04-26 23:47:44.073210 common_image_tools-0.1.6/common_image_tools/visualization.py
+-rw-r--r--   0        0        0      606 2024-05-10 11:44:34.865151 common_image_tools-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      832 2024-04-26 23:47:44.005195 common_image_tools-0.1.6/README.md
+-rw-r--r--   0        0        0     1548 1970-01-01 00:00:00.000000 common_image_tools-0.1.6/PKG-INFO
```

### Comparing `common_image_tools-0.1.5/common_image_tools/conversion.py` & `common_image_tools-0.1.6/common_image_tools/conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from typing import Tuple
+
 import cv2
 import dlib
 import numpy as np
 from PIL import Image
 
 
 # === PILLOW - OPENCV ==================================================================================================
@@ -45,30 +47,30 @@
 
     # Convert cv2 image to PIL image
     return Image.fromarray(cv2.cvtColor(cv2_image, cv2.COLOR_BGR2RGB))
 
 
 # === DLIB =============================================================================================================
 
-def rect_to_tuple(rect: dlib.rectangle) -> tuple[int, int, int, int]:
+def rect_to_tuple(rect: dlib.rectangle) -> Tuple[int, int, int, int]:
     """Convert a dlib rectangle object to a tuple representing a bounding box.
 
     This function takes a rectangle object representing a bounding box compatible with the dlib library
     and converts it into a tuple in the format (x, y, width, height).
 
     Parameters:
         rect (dlib.rectangle): A rectangle object representing the bounding box.
 
     Returns:
         tuple[int, int, int, int]: A tuple representing the bounding box in the format (x, y, width, height).
     """
     return rect.left(), rect.top(), rect.right() - rect.left(), rect.bottom() - rect.top()
 
 
-def tuple_to_rect(bbox: tuple) -> dlib.rectangle:
+def tuple_to_rect(bbox: Tuple) -> dlib.rectangle:
     """Convert a tuple representing a bounding box to a rectangle object.
 
     This function takes a tuple representing a bounding box in the format (x, y, width, height)
     and converts it into a rectangle object compatible with the dlib library.
 
     Parameters:
         bbox (tuple): A tuple representing the bounding box in the format (x, y, width, height).
```

### Comparing `common_image_tools-0.1.5/common_image_tools/operation.py` & `common_image_tools-0.1.6/common_image_tools/operation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 from math import ceil
+from typing import Tuple, List
 
 import cv2
 import numpy as np
 
 
-def resize_image_with_aspect_ratio(image: np.ndarray, size: tuple[int, int]) -> np.ndarray:
+def resize_image_with_aspect_ratio(image: np.ndarray, size: Tuple[int, int]) -> np.ndarray:
     height, width = size
 
     # Calculate the aspect ratio
     aspect_ratio = width / float(height)
 
     # Calculate new dimensions while preserving the aspect ratio
     if image.shape[1] / image.shape[0] > aspect_ratio:
@@ -23,15 +24,15 @@
     # Resize the image using the calculated dimensions
     resized_image = cv2.resize(image, (new_width, new_height))
 
     # Save the resized image
     return resized_image
 
 
-def is_point_in_bbox(point: tuple[int, int], bbox: tuple[int, int, int, int]) -> bool:
+def is_point_in_bbox(point: Tuple[int, int], bbox: Tuple[int, int, int, int]) -> bool:
     x1, y1, w, h = bbox
     x2, y2 = x1 + w, y1 + h
     x, y = point
     if x1 < x < x2 and y1 < y < y2:
         return True
     return False
 
@@ -43,25 +44,25 @@
     # When measureDist=false , the return value is +1, -1, and 0, respectively. Otherwise, the return value is a
     # signed distance between the point and the nearest contour edge.
     result = cv2.pointPolygonTest(ctn, point, measureDist=False)
 
     return result >= 0
 
 
-def scale_bboxes(bboxes: list[tuple], scale_factor: float) -> list[tuple]:
+def scale_bboxes(bboxes: List[Tuple], scale_factor: float) -> List[Tuple]:
     f_bboxes = []
     for box in bboxes:
         x, y, w, h = box
         f_bboxes.append(
             (ceil(x * scale_factor), ceil(y * scale_factor), ceil(w * scale_factor), ceil(h * scale_factor)))
 
     return f_bboxes
 
 
-def bbox_centroid(bbox: tuple[int, int, int, int]) -> tuple[int, int]:
+def bbox_centroid(bbox: Tuple[int, int, int, int]) -> Tuple[int, int]:
     """
     Calculate the centroid coordinates of a bounding box.
 
     Parameters:
         bbox (tuple): A tuple representing the bounding box in the format (x, y, width, height).
 
     Returns:
```

### Comparing `common_image_tools-0.1.5/common_image_tools/tool.py` & `common_image_tools-0.1.6/common_image_tools/tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from typing import Tuple
+
 import cv2
 import numpy as np
 from PIL import Image
 
 
 def opencv_built_with_gstreamer() -> bool:
     """Check if OpenCV has been built with GStreamer support.
@@ -128,30 +130,30 @@
     colored_image = cv2.bitwise_and(new_hsv_image, new_hsv_image, mask=mask)
     original_image = cv2.bitwise_and(image, image, mask=cv2.bitwise_not(mask))
     final_img = cv2.bitwise_xor(colored_image, original_image)
 
     return final_img
 
 
-def create_pil_image(size: tuple, color: tuple) -> Image:
+def create_pil_image(size: Tuple[int, int], color: Tuple[int, int, int]) -> Image:
     """Create a PIL image with the specified color and size.
 
     Args:
         size (tuple): Size of the image
         color (tuple): Color of the image in RGB format
 
     Returns:
         PIL.Image: Image in PIL format (RGB)
     """
     from PIL import Image
 
     return Image.new("RGB", size, color)
 
 
-def create_cv2_image(size: tuple[int, int], color: tuple[int, int, int]) -> np.ndarray:
+def create_cv2_image(size: Tuple[int, int], color: Tuple[int, int, int]) -> np.ndarray:
     """
     Creates a NumPy array representing an image using OpenCV conventions.
 
     Parameters:
         size (tuple[int, int]): A tuple specifying the dimensions of the image in the format (height, width).
         color (tuple[int, int, int]): A tuple representing the color of the image in BGR (Blue, Green, Red) format.
```

### Comparing `common_image_tools-0.1.5/common_image_tools/verification.py` & `common_image_tools-0.1.6/common_image_tools/verification.py`

 * *Files identical despite different names*

### Comparing `common_image_tools-0.1.5/pyproject.toml` & `common_image_tools-0.1.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "common-image-tools"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Federico Lanzani <federico@federicolanzani.com>"]
 readme = "README.md"
 packages = [{include = "common_image_tools"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pillow = ">=9.5.0"
 opencv-python = "~4.8.0.76"
 color-transfer = "^0.1"
 scikit-image = "^0.21.0"
-dlib = "^19.20.0"
+dlib = "19.24.2"
 
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 matplotlib = "^3.7.2"
 pre-commit = "^3.5.0"
 pytest = "^8.1.1"
```

### Comparing `common_image_tools-0.1.5/README.md` & `common_image_tools-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `common_image_tools-0.1.5/PKG-INFO` & `common_image_tools-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: common-image-tools
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Federico Lanzani
 Author-email: federico@federicolanzani.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: color-transfer (>=0.1,<0.2)
-Requires-Dist: dlib (>=19.20.0,<20.0.0)
+Requires-Dist: dlib (==19.24.2)
 Requires-Dist: opencv-python (>=4.8.0.76,<4.9.0.0)
 Requires-Dist: pillow (>=9.5.0)
 Requires-Dist: scikit-image (>=0.21.0,<0.22.0)
 Description-Content-Type: text/markdown
 
 # Common Image Tools
```

