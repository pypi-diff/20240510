# Comparing `tmp/data_transformation_wizzard-0.1.3.tar.gz` & `tmp/data_transformation_wizzard-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_transformation_wizzard-0.1.3.tar", max compression
+gzip compressed data, was "data_transformation_wizzard-0.1.4.tar", max compression
```

## Comparing `data_transformation_wizzard-0.1.3.tar` & `data_transformation_wizzard-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      441 2024-05-10 10:58:25.173994 data_transformation_wizzard-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1941 2024-05-09 10:48:48.395132 data_transformation_wizzard-0.1.3/README.md
--rw-r--r--   0        0        0      127 2024-05-09 11:06:49.013884 data_transformation_wizzard-0.1.3/src/data_transformation_wizzard/__init__.py
--rw-r--r--   0        0        0     2913 2024-05-09 20:18:30.684481 data_transformation_wizzard-0.1.3/src/data_transformation_wizzard/cross_correlation.py
--rw-r--r--   0        0        0     2288 2024-05-09 20:15:22.046267 data_transformation_wizzard-0.1.3/src/data_transformation_wizzard/time_series_windowing.py
--rw-r--r--   0        0        0     1294 2024-05-09 10:48:48.399873 data_transformation_wizzard-0.1.3/src/data_transformation_wizzard/transpose.py
--rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 data_transformation_wizzard-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      441 2024-05-10 18:53:09.055352 data_transformation_wizzard-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1941 2024-05-09 10:48:48.395132 data_transformation_wizzard-0.1.4/README.md
+-rw-r--r--   0        0        0      127 2024-05-09 11:06:49.013884 data_transformation_wizzard-0.1.4/src/data_transformation_wizzard/__init__.py
+-rw-r--r--   0        0        0     2615 2024-05-10 18:53:23.640692 data_transformation_wizzard-0.1.4/src/data_transformation_wizzard/cross_correlation.py
+-rw-r--r--   0        0        0     1896 2024-05-10 18:53:23.593066 data_transformation_wizzard-0.1.4/src/data_transformation_wizzard/time_series_windowing.py
+-rw-r--r--   0        0        0     1294 2024-05-09 10:48:48.399873 data_transformation_wizzard-0.1.4/src/data_transformation_wizzard/transpose.py
+-rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 data_transformation_wizzard-0.1.4/PKG-INFO
```

### Comparing `data_transformation_wizzard-0.1.3/README.md` & `data_transformation_wizzard-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `data_transformation_wizzard-0.1.3/src/data_transformation_wizzard/cross_correlation.py` & `data_transformation_wizzard-0.1.4/src/data_transformation_wizzard/cross_correlation.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 def convolution2d(
     input_matrix: list | np.ndarray, kernel: list | np.ndarray, stride: int = 1
 ) -> np.ndarray:
     """
     Apply 2D convolution to an input matrix with a given kernel and stride.
 
     Parameters:
-    input_matrix (Union[List[float], np.ndarray]): The 2D input matrix consisting of numbers.
-    kernel (Union[List[float], np.ndarray]): The kernel, a 2D array of real numbers.
+    input_matrix (list | np.ndarray): The 2D input matrix consisting of numbers.
+    kernel (list | np.ndarray): The kernel, a 2D array of real numbers.
     stride (int, optional): The stride, an integer that is greater than 0. Default is 1.
 
     Returns:
-    Union[np.ndarray, List[List[float]]]: The output matrix, either a 2D Numpy array or a list of lists, matching the input type.
+    output matrix (np.ndarray): The output matrix, either a 2D Numpy array or a list of lists, matching the input type.
 
     Raises:
     TypeError: If input_matrix or kernel is not a list or numpy array.
     ValueError: If input_matrix or kernel does not contain only integers or floats, or if stride is not a positive int.
     """
     if not isinstance(input_matrix, (list, np.ndarray)):
         raise TypeError("input_matrix must be a list or numpy array")
@@ -34,17 +34,14 @@
         for sublist in kernel
         for i in sublist
     ):
         raise ValueError("kernel must contain only numbers")
     if not isinstance(stride, int) or stride < 1:
         raise ValueError("stride must be a positive integer")
 
-    # Determine the output type based on the input type
-    output_type = np.ndarray if isinstance(input_matrix, np.ndarray) else list
-
     # Convert input_matrix and kernel to numpy arrays
     input_matrix = (
         np.array(input_matrix, dtype=float)
         if not isinstance(input_matrix, np.ndarray)
         else input_matrix
     )
     kernel = (
@@ -71,11 +68,8 @@
                 input_matrix[
                     i * stride : i * stride + x_kern,
                     j * stride : j * stride + y_kern,
                 ]
                 * kernel
             )
 
-    # Convert output to the same type as input
-    return (
-        output_matrix if output_type is np.ndarray else output_matrix.tolist()
-    )
+    return output_matrix
```

### Comparing `data_transformation_wizzard-0.1.3/src/data_transformation_wizzard/time_series_windowing.py` & `data_transformation_wizzard-0.1.4/src/data_transformation_wizzard/time_series_windowing.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 import numpy as np
 
 
 def window1d(
     input_array: list | np.ndarray, size: int, shift: int = 1, stride: int = 1
 ) -> list[list | np.ndarray]:
     """
-    This function performs a windowing operation on a 1-dimensional input array.
-    Parameters:
-    input_array (Union[List[float], np.ndarray]): The 1-dimensional input array consisting of numbers.
-    size (int): The size of each window. This must be a positive integer.
-    shift (int, optional): The number of positions to shift the window at each step. This must be a positive integer. Defaults to 1.
-    stride (int, optional): The number of positions to step within each window. This must be a positive integer. Defaults to 1.
+    Perform a windowing operation on a 1-dimensional input array.
+
+    Args:
+    input_array (list | np.ndarray): The 1-dimensional input array.
+    size (int): The size of each window.
+    shift (int, optional): The number of positions to shift the window at each step.
+    stride (int, optional): The number of positions to step within each window.
+
     Returns:
-    Union[List[Union[List[float], np.ndarray]], np.ndarray]: A list or numpy array of windows, matching the input format.
+    list[list | np.ndarray]: A list of windows, where each window is either a list or a numpy array.
+
     Raises:
     TypeError: If input_array is not a list or numpy array.
-    ValueError: If input_array does not contain only integers or floats, or if size, shift, or stride are not positive integers.
+    ValueError: If input_array does not contain only integers or floats.
     """
     if not isinstance(input_array, (list, np.ndarray)):
         raise TypeError("input_array must be a list or numpy array")
     if not all(isinstance(i, (int, float, np.number)) for i in input_array):
         raise ValueError("input_array must contain only numbers")
     if not isinstance(size, int) or size < 1:
         raise ValueError("size must be an integer greater than 0")
     if not isinstance(shift, int) or shift < 1:
         raise ValueError("shift must be an integer greater than 0")
     if not isinstance(stride, int) or stride < 1:
         raise ValueError("stride must be an integer greater than 0")
 
-    # Determine the output type based on the input type
-    output_type = np.ndarray if isinstance(input_array, np.ndarray) else list
-
-    # Convert input_array to numpy array
+    input_was_ndarray = isinstance(input_array, np.ndarray)
     input_array = np.array(input_array)
 
-    # Iterate over the input_array with a step size of shift
     output = []
     i = 0
     while i + (size - 1) * stride < len(input_array):
         window = input_array[i : i + (size - 1) * stride + 1 : stride]
         if len(window) == size:
-            output.append(window)
+            if input_was_ndarray:
+                output.append(window)
+            else:
+                output.append(window.tolist())
         i += shift
 
-    # Convert output to the same type as input
-    return output_type(output)
+    return output
```

### Comparing `data_transformation_wizzard-0.1.3/src/data_transformation_wizzard/transpose.py` & `data_transformation_wizzard-0.1.4/src/data_transformation_wizzard/transpose.py`

 * *Files identical despite different names*

### Comparing `data_transformation_wizzard-0.1.3/PKG-INFO` & `data_transformation_wizzard-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_transformation_wizzard
-Version: 0.1.3
+Version: 0.1.4
 Summary: Transpose.Windowing.Convolution
 License: Edgaras Gacionis
 Author: Edgaras Gacionis
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

