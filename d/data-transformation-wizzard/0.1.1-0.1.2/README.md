# Comparing `tmp/data_transformation_wizzard-0.1.1.tar.gz` & `tmp/data_transformation_wizzard-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_transformation_wizzard-0.1.1.tar", max compression
+gzip compressed data, was "data_transformation_wizzard-0.1.2.tar", max compression
```

## Comparing `data_transformation_wizzard-0.1.1.tar` & `data_transformation_wizzard-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      444 2024-05-08 22:39:58.172227 data_transformation_wizzard-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1941 2024-05-07 11:08:41.881080 data_transformation_wizzard-0.1.1/README.md
--rw-r--r--   0        0        0      127 2024-05-07 11:08:41.884358 data_transformation_wizzard-0.1.1/src/data_transformation_wizzard/__init__.py
--rw-r--r--   0        0        0     2785 2024-05-08 22:19:41.742323 data_transformation_wizzard-0.1.1/src/data_transformation_wizzard/cross_correlation.py
--rw-r--r--   0        0        0     2269 2024-05-08 22:19:41.726657 data_transformation_wizzard-0.1.1/src/data_transformation_wizzard/time_series_windowing.py
--rw-r--r--   0        0        0     1294 2024-05-08 22:19:41.742323 data_transformation_wizzard-0.1.1/src/data_transformation_wizzard/transpose.py
--rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 data_transformation_wizzard-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      441 2024-05-09 19:09:53.046439 data_transformation_wizzard-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1941 2024-05-09 10:48:48.395132 data_transformation_wizzard-0.1.2/README.md
+-rw-r--r--   0        0        0      127 2024-05-09 11:06:49.013884 data_transformation_wizzard-0.1.2/src/data_transformation_wizzard/__init__.py
+-rw-r--r--   0        0        0     2785 2024-05-09 10:48:48.398419 data_transformation_wizzard-0.1.2/src/data_transformation_wizzard/cross_correlation.py
+-rw-r--r--   0        0        0     2277 2024-05-09 19:35:09.628681 data_transformation_wizzard-0.1.2/src/data_transformation_wizzard/time_series_windowing.py
+-rw-r--r--   0        0        0     1294 2024-05-09 10:48:48.399873 data_transformation_wizzard-0.1.2/src/data_transformation_wizzard/transpose.py
+-rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 data_transformation_wizzard-0.1.2/PKG-INFO
```

### Comparing `data_transformation_wizzard-0.1.1/README.md` & `data_transformation_wizzard-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `data_transformation_wizzard-0.1.1/src/data_transformation_wizzard/cross_correlation.py` & `data_transformation_wizzard-0.1.2/src/data_transformation_wizzard/cross_correlation.py`

 * *Files identical despite different names*

### Comparing `data_transformation_wizzard-0.1.1/src/data_transformation_wizzard/time_series_windowing.py` & `data_transformation_wizzard-0.1.2/src/data_transformation_wizzard/time_series_windowing.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,24 @@
 
 
 def window1d(
     input_array: list | np.ndarray, size: int, shift: int = 1, stride: int = 1
 ) -> list[list | np.ndarray]:
     """
     This function performs a windowing operation on a 1-dimensional input array.
-
     Parameters:
     input_array (Union[List[float], np.ndarray]): The 1-dimensional input array consisting of numbers.
     size (int): The size of each window. This must be a positive integer.
     shift (int, optional): The number of positions to shift the window at each step. This must be a positive integer. Defaults to 1.
     stride (int, optional): The number of positions to step within each window. This must be a positive integer. Defaults to 1.
-
     Returns:
     List[Union[List[float], np.ndarray]]: A list of numpy arrays, where each array is a window in the original array.
-
     Raises:
     TypeError: If input_array is not a list or numpy array.
     ValueError: If input_array does not contain only integers or floats, or if size, shift, or stride are not positive integers.
-
     Example:
     >>> window1d([1, 2, 3, 4, 5, 6, 7, 8, 9, 10], 5, 2, 2)
     [array([1., 3., 5.]), array([3., 5., 7.]), array([5., 7., 9.])]
     """
     # Input validation
     if not isinstance(input_array, (list, np.ndarray)):
         raise TypeError("input_array must be a list or numpy array")
@@ -35,17 +31,18 @@
         raise ValueError("shift must be an integer greater than 0")
     if not isinstance(stride, int) or stride < 1:
         raise ValueError("stride must be an integer greater than 0")
 
     # Convert input_array to numpy array if it's not
     input_array = np.array(input_array, dtype=float)
 
-    # Initialize the output list
     output = []
+    i = 0
 
     # Iterate over the input_array with a step size of shift
-    for i in range(0, len(input_array) - size + 1, shift):
-        window = input_array[i : i + size : stride]
-        output.append(window)
+    while i + (size - 1) * stride < len(input_array):
+        window = input_array[i: i + (size - 1) * stride + 1: stride]
+        if len(window) == size:
+            output.append(window)
+        i += shift
 
-    # Return the output list
     return output
```

### Comparing `data_transformation_wizzard-0.1.1/src/data_transformation_wizzard/transpose.py` & `data_transformation_wizzard-0.1.2/src/data_transformation_wizzard/transpose.py`

 * *Files identical despite different names*

### Comparing `data_transformation_wizzard-0.1.1/PKG-INFO` & `data_transformation_wizzard-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: data_transformation_wizzard
-Version: 0.1.1
+Version: 0.1.2
 Summary: Transpose.Windowing.Convolution
 License: Edgaras Gacionis
 Author: Edgaras Gacionis
-Requires-Python: ==3.11.5
+Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: numpy (>=1.26,<2.0)
 Description-Content-Type: text/markdown
 
 
 # Data Wizzard Library
 
 ## Overview
 The Data Wizzard Library is a Python package designed to simplify and streamline data transformation tasks. It provides a set of functions that perform common operations such as 2D transposition, 1D windowing, and 2D convolution. These functions are optimized for performance and ease of use, making it easier to manipulate and analyze data in Python.
```

