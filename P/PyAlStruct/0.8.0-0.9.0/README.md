# Comparing `tmp/PyAlStruct-0.8.0.tar.gz` & `tmp/pyalstruct-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAlStruct-0.8.0.tar", last modified: Tue Oct  3 21:29:30 2023, max compression
+gzip compressed data, was "pyalstruct-0.9.0.tar", last modified: Wed May  8 22:21:37 2024, max compression
```

## Comparing `PyAlStruct-0.8.0.tar` & `pyalstruct-0.9.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-10-03 21:29:30.027411 PyAlStruct-0.8.0/
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1073 2023-08-30 21:44:09.000000 PyAlStruct-0.8.0/LICENSE
--rw-r--r--   0 fathi     (1000) fathi     (1000)      847 2023-10-03 21:29:30.027411 PyAlStruct-0.8.0/PKG-INFO
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-10-03 21:29:30.022411 PyAlStruct-0.8.0/PyAlStruct.egg-info/
--rw-r--r--   0 fathi     (1000) fathi     (1000)      847 2023-10-03 21:29:29.000000 PyAlStruct-0.8.0/PyAlStruct.egg-info/PKG-INFO
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1045 2023-10-03 21:29:29.000000 PyAlStruct-0.8.0/PyAlStruct.egg-info/SOURCES.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)        1 2023-10-03 21:29:29.000000 PyAlStruct-0.8.0/PyAlStruct.egg-info/dependency_links.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)       10 2023-10-03 21:29:29.000000 PyAlStruct-0.8.0/PyAlStruct.egg-info/top_level.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)       13 2023-08-30 20:47:05.000000 PyAlStruct-0.8.0/README.md
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-10-03 21:29:30.022411 PyAlStruct-0.8.0/al_struct/
--rw-r--r--   0 fathi     (1000) fathi     (1000)        0 2023-08-30 20:40:14.000000 PyAlStruct-0.8.0/al_struct/__init__.py
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-10-03 21:29:30.022411 PyAlStruct-0.8.0/al_struct/algorithms/
--rw-r--r--   0 fathi     (1000) fathi     (1000)        0 2023-08-30 20:40:32.000000 PyAlStruct-0.8.0/al_struct/algorithms/__init__.py
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-10-03 21:29:30.023411 PyAlStruct-0.8.0/al_struct/algorithms/search/
--rw-r--r--   0 fathi     (1000) fathi     (1000)      122 2023-09-25 19:20:22.000000 PyAlStruct-0.8.0/al_struct/algorithms/search/__init__.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     2449 2023-10-03 21:28:21.000000 PyAlStruct-0.8.0/al_struct/algorithms/search/binary_search.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1297 2023-09-18 21:15:09.000000 PyAlStruct-0.8.0/al_struct/algorithms/search/linear_search.py
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-10-03 21:29:30.024411 PyAlStruct-0.8.0/al_struct/algorithms/sort/
--rw-r--r--   0 fathi     (1000) fathi     (1000)      244 2023-10-03 19:14:52.000000 PyAlStruct-0.8.0/al_struct/algorithms/sort/__init__.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1153 2023-09-25 22:02:55.000000 PyAlStruct-0.8.0/al_struct/algorithms/sort/bubble.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)      877 2023-09-25 22:04:26.000000 PyAlStruct-0.8.0/al_struct/algorithms/sort/insertion.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1349 2023-10-03 19:14:52.000000 PyAlStruct-0.8.0/al_struct/algorithms/sort/merge.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1259 2023-10-03 19:46:11.000000 PyAlStruct-0.8.0/al_struct/algorithms/sort/quick.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1002 2023-09-25 22:02:55.000000 PyAlStruct-0.8.0/al_struct/algorithms/sort/selection.py
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-10-03 21:29:30.024411 PyAlStruct-0.8.0/al_struct/data_structures/
--rw-r--r--   0 fathi     (1000) fathi     (1000)        0 2023-08-30 20:40:48.000000 PyAlStruct-0.8.0/al_struct/data_structures/__init__.py
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-10-03 21:29:30.024411 PyAlStruct-0.8.0/al_struct/data_structures/lists/
--rw-r--r--   0 fathi     (1000) fathi     (1000)       79 2023-09-08 23:42:59.000000 PyAlStruct-0.8.0/al_struct/data_structures/lists/__init__.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     4611 2023-10-03 21:28:21.000000 PyAlStruct-0.8.0/al_struct/data_structures/lists/singly_linked_list.py
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-10-03 21:29:30.025411 PyAlStruct-0.8.0/al_struct/data_structures/queues/
--rw-r--r--   0 fathi     (1000) fathi     (1000)       45 2023-09-08 23:42:59.000000 PyAlStruct-0.8.0/al_struct/data_structures/queues/__init__.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     2439 2023-10-03 21:28:21.000000 PyAlStruct-0.8.0/al_struct/data_structures/queues/queue.py
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-10-03 21:29:30.025411 PyAlStruct-0.8.0/al_struct/data_structures/stacks/
--rw-r--r--   0 fathi     (1000) fathi     (1000)       45 2023-09-08 23:42:59.000000 PyAlStruct-0.8.0/al_struct/data_structures/stacks/__init__.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     2459 2023-10-03 21:28:21.000000 PyAlStruct-0.8.0/al_struct/data_structures/stacks/stack.py
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-10-03 21:29:30.026411 PyAlStruct-0.8.0/al_struct/data_structures/trees/
--rw-r--r--   0 fathi     (1000) fathi     (1000)       66 2023-09-15 14:17:31.000000 PyAlStruct-0.8.0/al_struct/data_structures/trees/__init__.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     5716 2023-10-03 21:28:21.000000 PyAlStruct-0.8.0/al_struct/data_structures/trees/bst.py
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-10-03 21:29:30.026411 PyAlStruct-0.8.0/al_struct/utils/
--rw-r--r--   0 fathi     (1000) fathi     (1000)      954 2023-09-15 15:42:50.000000 PyAlStruct-0.8.0/al_struct/utils/__init__.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)      496 2023-09-02 21:50:35.000000 PyAlStruct-0.8.0/al_struct/utils/exceptions.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     3651 2023-09-15 16:07:41.000000 PyAlStruct-0.8.0/al_struct/utils/nodes.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)       38 2023-10-03 21:29:30.027411 PyAlStruct-0.8.0/setup.cfg
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1411 2023-10-03 21:28:21.000000 PyAlStruct-0.8.0/setup.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-05-08 22:21:37.730177 pyalstruct-0.9.0/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1073 2024-02-28 20:34:35.000000 pyalstruct-0.9.0/LICENSE
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      847 2024-05-08 22:21:37.729177 pyalstruct-0.9.0/PKG-INFO
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-05-08 22:21:37.729177 pyalstruct-0.9.0/PyAlStruct.egg-info/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      847 2024-05-08 22:21:37.000000 pyalstruct-0.9.0/PyAlStruct.egg-info/PKG-INFO
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1043 2024-05-08 22:21:37.000000 pyalstruct-0.9.0/PyAlStruct.egg-info/SOURCES.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)        1 2024-05-08 22:21:37.000000 pyalstruct-0.9.0/PyAlStruct.egg-info/dependency_links.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       10 2024-05-08 22:21:37.000000 pyalstruct-0.9.0/PyAlStruct.egg-info/top_level.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       13 2024-02-28 20:34:35.000000 pyalstruct-0.9.0/README.md
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-05-08 22:21:37.718177 pyalstruct-0.9.0/al_struct/
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-05-08 22:21:37.720177 pyalstruct-0.9.0/al_struct/algorithms/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)        0 2024-02-28 20:34:35.000000 pyalstruct-0.9.0/al_struct/algorithms/__init__.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-05-08 22:21:37.721177 pyalstruct-0.9.0/al_struct/algorithms/search/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      122 2024-02-28 20:34:35.000000 pyalstruct-0.9.0/al_struct/algorithms/search/__init__.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     2514 2024-05-08 22:19:03.000000 pyalstruct-0.9.0/al_struct/algorithms/search/binary_search.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1356 2024-05-08 22:19:03.000000 pyalstruct-0.9.0/al_struct/algorithms/search/linear_search.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-05-08 22:21:37.723177 pyalstruct-0.9.0/al_struct/algorithms/sort/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      244 2024-02-28 20:34:35.000000 pyalstruct-0.9.0/al_struct/algorithms/sort/__init__.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1207 2024-05-08 22:19:03.000000 pyalstruct-0.9.0/al_struct/algorithms/sort/bubble.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      926 2024-05-08 22:19:03.000000 pyalstruct-0.9.0/al_struct/algorithms/sort/insertion.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1439 2024-05-08 22:19:03.000000 pyalstruct-0.9.0/al_struct/algorithms/sort/merge.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1337 2024-05-08 22:19:03.000000 pyalstruct-0.9.0/al_struct/algorithms/sort/quick.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1051 2024-05-08 22:19:03.000000 pyalstruct-0.9.0/al_struct/algorithms/sort/selection.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-05-08 22:21:37.724177 pyalstruct-0.9.0/al_struct/data_structures/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)        0 2024-02-28 20:34:35.000000 pyalstruct-0.9.0/al_struct/data_structures/__init__.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-05-08 22:21:37.724177 pyalstruct-0.9.0/al_struct/data_structures/lists/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       79 2024-02-28 20:34:35.000000 pyalstruct-0.9.0/al_struct/data_structures/lists/__init__.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     4720 2024-05-08 22:03:03.000000 pyalstruct-0.9.0/al_struct/data_structures/lists/singly_linked_list.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-05-08 22:21:37.725177 pyalstruct-0.9.0/al_struct/data_structures/queues/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       45 2024-02-28 20:34:35.000000 pyalstruct-0.9.0/al_struct/data_structures/queues/__init__.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     2491 2024-05-08 22:03:03.000000 pyalstruct-0.9.0/al_struct/data_structures/queues/queue.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-05-08 22:21:37.726177 pyalstruct-0.9.0/al_struct/data_structures/stacks/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       45 2024-02-28 20:34:35.000000 pyalstruct-0.9.0/al_struct/data_structures/stacks/__init__.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     2511 2024-05-08 22:03:03.000000 pyalstruct-0.9.0/al_struct/data_structures/stacks/stack.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-05-08 22:21:37.726177 pyalstruct-0.9.0/al_struct/data_structures/trees/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       66 2024-02-28 20:34:35.000000 pyalstruct-0.9.0/al_struct/data_structures/trees/__init__.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     5930 2024-05-08 22:03:03.000000 pyalstruct-0.9.0/al_struct/data_structures/trees/bst.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-05-08 22:21:37.728177 pyalstruct-0.9.0/al_struct/utils/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      954 2024-02-28 20:34:35.000000 pyalstruct-0.9.0/al_struct/utils/__init__.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      496 2024-02-28 20:34:35.000000 pyalstruct-0.9.0/al_struct/utils/exceptions.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     3797 2024-05-08 22:19:03.000000 pyalstruct-0.9.0/al_struct/utils/nodes.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       38 2024-05-08 22:21:37.730177 pyalstruct-0.9.0/setup.cfg
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1411 2024-05-08 22:19:03.000000 pyalstruct-0.9.0/setup.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-05-08 22:21:37.729177 pyalstruct-0.9.0/tests/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1706 2024-02-28 20:34:35.000000 pyalstruct-0.9.0/tests/test_nodes.py
```

### Comparing `PyAlStruct-0.8.0/LICENSE` & `pyalstruct-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyAlStruct-0.8.0/PKG-INFO` & `pyalstruct-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAlStruct
-Version: 0.8.0
+Version: 0.9.0
 Summary: Implementation of data structures and algorithms in python
 Home-page: https://github.com/fathiabdelmalek/PyAlStruct
 Author: Fathi Abdelmalek
 Author-email: abdelmalek.fathi.2001@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
```

### Comparing `PyAlStruct-0.8.0/PyAlStruct.egg-info/PKG-INFO` & `pyalstruct-0.9.0/PyAlStruct.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAlStruct
-Version: 0.8.0
+Version: 0.9.0
 Summary: Implementation of data structures and algorithms in python
 Home-page: https://github.com/fathiabdelmalek/PyAlStruct
 Author: Fathi Abdelmalek
 Author-email: abdelmalek.fathi.2001@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
```

### Comparing `PyAlStruct-0.8.0/PyAlStruct.egg-info/SOURCES.txt` & `pyalstruct-0.9.0/PyAlStruct.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
 setup.py
 PyAlStruct.egg-info/PKG-INFO
 PyAlStruct.egg-info/SOURCES.txt
 PyAlStruct.egg-info/dependency_links.txt
 PyAlStruct.egg-info/top_level.txt
-al_struct/__init__.py
 al_struct/algorithms/__init__.py
 al_struct/algorithms/search/__init__.py
 al_struct/algorithms/search/binary_search.py
 al_struct/algorithms/search/linear_search.py
 al_struct/algorithms/sort/__init__.py
 al_struct/algorithms/sort/bubble.py
 al_struct/algorithms/sort/insertion.py
@@ -23,8 +22,9 @@
 al_struct/data_structures/queues/queue.py
 al_struct/data_structures/stacks/__init__.py
 al_struct/data_structures/stacks/stack.py
 al_struct/data_structures/trees/__init__.py
 al_struct/data_structures/trees/bst.py
 al_struct/utils/__init__.py
 al_struct/utils/exceptions.py
-al_struct/utils/nodes.py
+al_struct/utils/nodes.py
+tests/test_nodes.py
```

### Comparing `PyAlStruct-0.8.0/al_struct/algorithms/search/binary_search.py` & `pyalstruct-0.9.0/al_struct/algorithms/search/binary_search.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,36 @@
+from typing import Any
+
 from al_struct.algorithms.sort import *
 
 
 class BinarySearch:
     """
     Apply binary search for a target in an array.
     Default sort algorithm is selection sort.
     """
-    def __init__(self, array, sort='quick'):
+    def __init__(self, array: Any, sort: str = 'quick'):
         match sort:
             case 'selection':
                 self._sort = SelectionSort()
             case 'insertion':
                 self._sort = InsertionSort()
             case 'bubble':
                 self._sort = BubbleSort()
             case 'merge':
                 self._sort = MergeSort()
             case 'quick':
                 self._sort = QuickSort()
         self._array = self._sort.sort(array)
 
     @property
-    def array(self):
+    def array(self) -> Any:
         return self._array
 
-    def exists(self, target) -> bool:
+    def exists(self, target: Any) -> bool:
         """
         Return boolean value about the existence of the target.
         :param target: The target to search for.
         :return: bool -- True if target exists, otherwise False.
         """
         left, right = 0, len(self._array) - 1
         while left <= right:
@@ -37,15 +39,15 @@
                 return True
             elif self._array[mid] < target:
                 left = mid + 1
             else:
                 right = mid - 1
         return False
 
-    def find_index(self, target) -> int:
+    def find_index(self, target: Any) -> int:
         """
         Return the index of target if exists in the array.
         :param target: The target to search for.
         :return: int -- The index of target if exists, otherwise return '-1'.
         """
         left, right = 0, len(self._array) - 1
         while left <= right:
@@ -54,15 +56,15 @@
                 return self._array.index(mid)
             elif self._array[mid] < target:
                 left = mid + 1
             else:
                 right = mid - 1
         return -1
 
-    def find_element(self, target):
+    def find_element(self, target: Any) -> Any:
         """
         Return the element if exists in the array.
         :param target: The target to search for.
         :return: The element if exists, otherwise 'None'.
         """
         left, right = 0, len(self._array) - 1
         while left <= right:
```

### Comparing `PyAlStruct-0.8.0/al_struct/algorithms/search/linear_search.py` & `pyalstruct-0.9.0/al_struct/algorithms/search/linear_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,44 @@
+from typing import Any
+
+
 class LinearSearch:
     """
     Apply linear search for a target in an array.
     """
-    def __init__(self, array):
+    def __init__(self, array: Any):
         self._array = array
 
     @property
-    def array(self):
+    def array(self) -> Any:
         return self._array
 
-    def exists(self, target) -> bool:
+    def exists(self, target: Any) -> bool:
         """
         Return boolean value about the existence of the target.
         :param target: The target to search for.
         :return: bool -- True if target exists, otherwise False.
         """
         for element in self._array:
             if element == target:
                 return True
         return False
 
-    def find_index(self, target) -> int:
+    def find_index(self, target: Any) -> int:
         """
         Return the index of target if exists in the array.
         :param target: The target to search for.
         :return: int -- The index of target if exists, otherwise return '-1'.
         """
         for element in self._array:
             if element == target:
                 return self._array.index(target)
         return -1
 
-    def find_element(self, target):
+    def find_element(self, target: Any) -> Any:
         """
         Return the element if exists in the array.
         :param target: The target to search for.
         :return: The element if exists, otherwise 'None'.
         """
         for element in self._array:
             if element == target:
```

### Comparing `PyAlStruct-0.8.0/al_struct/algorithms/sort/bubble.py` & `pyalstruct-0.9.0/al_struct/algorithms/sort/bubble.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from typing import Any, List
+
+
 class BubbleSort:
-    def sort(self, arr):
+    def sort(self, arr: iter(Any)) -> iter(Any):
         """
         Perform bubble sort on the input list 'arr' in-place.
 
         :param arr: The input list to be sorted.
         :return: arr -- The sorted array.
         """
         n = len(arr)
         sorted_arr = arr.copy()
 
         for i in range(n - 1):
             # Flag to check if any swaps were made in this pass
             swapped = False
-
             # Last i elements are already in place, so we don't need to check them
             for j in range(0, n - i - 1):
                 if sorted_arr[j] > sorted_arr[j + 1]:
                     # Swap arr[j] and arr[j+1]
                     sorted_arr[j], sorted_arr[j + 1] = sorted_arr[j + 1], sorted_arr[j]
                     swapped = True
```

### Comparing `PyAlStruct-0.8.0/al_struct/algorithms/sort/insertion.py` & `pyalstruct-0.9.0/al_struct/algorithms/sort/insertion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from typing import Any
+
+
 class InsertionSort:
-    def sort(self, arr):
+    def sort(self, arr: iter(Any)) -> iter(Any):
         """
         Perform insertion sort on the input list 'arr' in-place.
 
         :param arr: The input list to be sorted.
         :return: arr -- The sorted array.
         """
         sorted_arr = arr.copy()
```

### Comparing `PyAlStruct-0.8.0/al_struct/algorithms/sort/merge.py` & `pyalstruct-0.9.0/al_struct/algorithms/sort/merge.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from typing import Any
+
+
 class MergeSort:
-    def _merge(self, arr, left_side, right_side):
+    def _merge(self, arr: iter(Any), left_side: iter(Any), right_side: iter(Any)) -> None:
         i, j, k = 0, 0, 0
         while i < len(left_side) and j < len(right_side):
             if left_side[i] < right_side[j]:
                 arr[k] = left_side[i]
                 i += 1
             else:
                 arr[k] = right_side[j]
@@ -14,15 +17,15 @@
             i += 1
             k += 1
         while j < len(right_side):
             arr[k] = right_side[j]
             j += 1
             k += 1
 
-    def sort(self, arr):
+    def sort(self, arr: iter(Any)) -> iter(Any):
         """
         Perform quick sort on the input list 'arr' in-place.
 
         :param arr: The input list to be sorted.
         :return: arr -- The sorted array.
         """
         sorted_arr = arr.copy()
```

### Comparing `PyAlStruct-0.8.0/al_struct/algorithms/sort/selection.py` & `pyalstruct-0.9.0/al_struct/algorithms/sort/selection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from typing import Any
+
+
 class SelectionSort:
-    def sort(self, arr):
+    def sort(self, arr: iter(Any)) -> iter(Any):
         """
         Perform selection sort on the input list 'arr' in-place.
 
         :param arr: The input list to be sorted.
         :return: arr -- The sorted array.
         """
         n = len(arr)
```

### Comparing `PyAlStruct-0.8.0/al_struct/data_structures/lists/singly_linked_list.py` & `pyalstruct-0.9.0/al_struct/data_structures/lists/singly_linked_list.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from utils.exceptions import NodeNotFoundException, EmptyListException
+from typing import Any
+
+from al_struct.utils.exceptions import NodeNotFoundException, EmptyListException
 from al_struct.utils.nodes import Node
 
 
 class SinglyLinkedList:
     """Singly linked list data structure."""
 
     def __init__(self):
@@ -47,85 +49,85 @@
     def is_empty(self) -> bool:
         """
         Check if the linked list is empty.
         :returns: bool -- True if the linked list is empty, otherwise False.
         """
         return self._head is None
 
-    def prepend(self, data):
+    def prepend(self, data: Any) -> None:
         """
         Add a new node with data to the beginning of the list.
         :param data: The data to be added to the list.
         """
         node = Node(data)
         node.next = self._head
         self._head = node
 
-    def append(self, data):
+    def append(self, data: Any) -> None:
         """
         Add a new node with data to the end of the list.
         :param data: The data to be added to the list.
         """
         node = Node(data)
         if not self._head:
             self._head = node
             return
         temp = self._head
         while temp.next:
             temp = temp.next
         temp.next = node
 
-    def get_head(self):
+    def get_head(self) -> Any:
         """
         Get data of the first node in the list.
         :return: The data of the first node in the list.
         """
         if not self._head:
             raise EmptyListException()
         return self._head.key
 
-    def get_tail(self):
+    def get_tail(self) -> Any:
         """
         Get data of the last node in the list.
         :return: The data of the last node in the list.
         """
         if not self._head:
             raise EmptyListException()
         temp = self._head
         while temp.next:
             temp = temp.next
         return temp.key
 
-    def get(self, data):
+    def get(self, data: Any) -> Any:
         """
         Return the node that contains data if exist in the list.
         :param data: The data to search for.
         :return: Node -- The node that contains data if exists, otherwise None.
         """
         temp = self._head
         while temp:
             if temp.key == data:
                 return temp
             temp = temp.next
         return None
 
-    def search(self, data) -> bool:
+    def search(self, data: Any) -> bool:
         """
         Return boolean value if data exists in the list.
         :param data: The data to search for.
         :return: bool -- True if data exists, otherwise False.
         """
         temp = self._head
         while temp:
             if temp.key == data:
                 return True
             temp = temp.next
         return False
 
-    def index(self, data) -> int:
+    def index(self, data: Any) -> int:
         """
         Find the index of the first occurrence of data in the linked list.
         :param data: The data to search for in the list.
         :returns: int -- The index of the first occurrence of the data.
         :raises NodeNotFoundException: If the data is not found in the linked list.
         """
         index = 0
@@ -133,15 +135,15 @@
         while temp:
             if temp.key == data:
                 return index
             temp = temp.next
             index += 1
         raise NodeNotFoundException(data)
 
-    def delete(self, data):
+    def delete(self, data: Any) -> None:
         """
         Delete the first occurrence of data in the linked list.
         :param data: The data to be deleted
         """
         if not self._head:
             raise EmptyListException()
         if self._head.key == data:
```

### Comparing `PyAlStruct-0.8.0/al_struct/data_structures/queues/queue.py` & `pyalstruct-0.9.0/al_struct/data_structures/queues/queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any
+
 from utils.exceptions import EmptyQueueException
 from al_struct.utils.nodes import Node
 
 
 class Queue:
     """Simple queue data structure."""
 
@@ -47,28 +49,28 @@
     def is_empty(self) -> bool:
         """
         Check if the queue is empty.
         :returns: bool -- True if the queue is empty, otherwise False.
         """
         return self._front is None
 
-    def enqueue(self, item):
+    def enqueue(self, item: Any) -> None:
         """
         Add a new node with item to the back of the queue.
         :param item: The item to be added to the queue.
         """
         node = Node(item)
         if self._front is None:
             self._front = node
             self._back = node
             return
         self._back.next = node
         self._back = node
 
-    def dequeue(self):
+    def dequeue(self) -> None:
         """
         Removes and returns an item from the front of the queue.
         :return: The item at the front of the queue if exists.
         :raise EmptyQueueException: If the stack is empty.
         """
         if self._front is None:
             raise EmptyQueueException()
@@ -76,15 +78,15 @@
             self._front = None
         data = self._front.data
         temp = self._front
         self._front = self._front.next
         del temp
         return data
 
-    def size(self):
+    def size(self) -> int:
         """
         Return The size of the queue.
         :return: int -- The size of the queue.
         """
         size = 0
         tmep = self._front
         while tmep:
```

### Comparing `PyAlStruct-0.8.0/al_struct/data_structures/stacks/stack.py` & `pyalstruct-0.9.0/al_struct/data_structures/stacks/stack.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any
+
 from utils.exceptions import EmptyStackException
 from al_struct.utils.nodes import Node
 
 
 class Stack:
     """Simple stack data structure."""
 
@@ -46,38 +48,38 @@
     def is_empty(self) -> bool:
         """
         Check if the stack is empty.
         :returns: bool -- True if the stack is empty, otherwise False.
         """
         return self._top is None
 
-    def push(self, item):
+    def push(self, item: Any) -> None:
         """
         Add a new item to the top of the stack.
         :param item: The item to be added to the stack.
         """
         node = Node(item)
         node.next = self._top
         self._top = node
 
-    def pop(self):
+    def pop(self) -> None:
         """
         Removes and returns an item from the top of the stack.
         :return: The item at the top of the stack if exists.
         :raise EmptyStackException: If the stack is empty.
         """
         if not self._top:
             raise EmptyStackException()
         item = self._top.key
         temp = self._top
         self._top = self._top.next
         del temp
         return item
 
-    def peek(self):
+    def peek(self) -> Any:
         """
         Return the item in the top of the stack without removing it.
         :return: The item of the node at the top of the stack.
         """
         if not self._top:
             raise EmptyStackException()
         return self._top.key
```

### Comparing `PyAlStruct-0.8.0/al_struct/data_structures/trees/bst.py` & `pyalstruct-0.9.0/al_struct/data_structures/trees/bst.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any
+
 from al_struct.utils.nodes import TreeNode
 
 
 class BinarySearchTree:
     """Binary search tree key structure."""
     def __init__(self):
         """Initialize an empty binary search tree."""
@@ -39,25 +41,25 @@
         def _height(node):
             if node is None:
                 return 0
             return 1 + max(_height(node.left), _height(node.right))
         return _height(self._root)
 
     @property
-    def min(self):
+    def min(self) -> Any:
         """
         Returns the minimum value in the tree.
         """
         temp = self._root
         while temp.left:
             temp = temp.left
         return temp.key
 
     @property
-    def max(self):
+    def max(self) -> Any:
         """
         Returns the maximum value in the tree.
         """
         temp = self._root
         while temp.right:
             temp = temp.right
         return temp.key
@@ -65,122 +67,124 @@
     def is_empty(self) -> bool:
         """
         Check if the tree is empty.
         :returns: bool -- True if the tree is empty, otherwise False.
         """
         return self._root is None
 
-    def pre_order(self):
+    def pre_order(self) -> None:
         """
         Perform a preorder traversal of the binary search tree.
         """
         def _pre_order(node):
             if node:
                 print(node.key, end=', ')
                 _pre_order(node.left)
                 _pre_order(node.right)
         if self._root is not None:
             _pre_order(self._root)
             print("end")
 
-    def in_order(self):
+    def in_order(self) -> None:
         """
         Perform an inorder traversal of the binary search tree.
         """
         def _in_order(node):
             if node:
                 _in_order(node.left)
                 print(node.key, end=', ')
                 _in_order(node.right)
         if self._root is not None:
             _in_order(self._root)
             print("end")
 
-    def post_order(self):
+    def post_order(self) -> None:
         """
         Perform a postorder traversal of the binary search tree.
         """
         def _post_order(node):
             if node:
                 _post_order(node.left)
                 _post_order(node.right)
                 print(node.key, end=', ')
         if self._root is not None:
             _post_order(self._root)
             print("end")
 
-    def insert(self, key):
+    def insert(self, key: Any) -> None:
         """
         Insert new key to the tree if it's not exist.
         :param key: the key to be inserted.
         """
-        def _insert(root, key):
+        def _insert(root, _key) -> TreeNode:
             if root is None:
-                return TreeNode(key)
-            if key < root.key:
-                node = _insert(root.left, key)
+                return TreeNode(_key)
+            if _key == root.key:
+                raise ValueError(f'Key {_key} already exists')
+            if _key < root.key:
+                node = _insert(root.left, _key)
                 root.left = node
                 return root
-            node = _insert(root.right, key)
+            node = _insert(root.right, _key)
             root.right = node
             return root
         self._root = _insert(self._root, key)
         self._number_of_nodes += 1
 
-    def get(self, key) -> 'TreeNode':
+    def get(self, key) -> TreeNode:
         """
         Return the node that contains key if exist in the tree.
         :param key: The key to search for.
         :return: TreeNode -- The node that contains key if exists, otherwise None.
         """
-        def _search(root, key):
+        def _search(root, _key):
             if root is None:
                 return None
-            if root.key == key:
+            if root.key == _key:
                 return root
-            if key < root.key:
-                return _search(root.left, key)
-            return _search(root.right, key)
+            if _key < root.key:
+                return _search(root.left, _key)
+            return _search(root.right, _key)
         return _search(self._root, key)
 
     def search(self, key) -> bool:
         """
         Search for a key in the tree.
         :param key: The key to search for.
         :return: bool -- True if key exists in the tree, otherwise False.
         """
-        def _search(root, key):
+        def _search(root, _key):
             if root is None:
                 return False
-            if root.key == key:
+            if root.key == _key:
                 return True
-            if key < root.key:
-                return _search(root.left, key)
-            return _search(root.right, key)
+            if _key < root.key:
+                return _search(root.left, _key)
+            return _search(root.right, _key)
         if self.is_empty():
             return False
         return _search(self._root, key)
 
-    def delete(self, key):
+    def delete(self, key: Any) -> None:
         """
         Delete a key from the tree.
         :param key: The key to be added.
         """
         def _min_value_node(node):
             while node.left is not None:
                 node = node.left
             return node
 
-        def _delete(root, key):
+        def _delete(root, _key):
             if root is None:
                 return root
-            if key < root.key:
-                root.left = _delete(root.left, key)
-            elif key > root.key:
-                root.right = _delete(root.right, key)
+            if _key < root.key:
+                root.left = _delete(root.left, _key)
+            elif _key > root.key:
+                root.right = _delete(root.right, _key)
             else:
                 if root.left is None:
                     return root.right
                 elif root.right is None:
                     return root.left
                 root.key = _min_value_node(root.right).key
                 root.right = _delete(root.right, root.key)
```

### Comparing `PyAlStruct-0.8.0/al_struct/utils/__init__.py` & `pyalstruct-0.9.0/al_struct/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAlStruct-0.8.0/al_struct/utils/nodes.py` & `pyalstruct-0.9.0/al_struct/utils/nodes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,49 @@
+from typing import Any
+
+
 class Node:
     """Basic node for linked data structures."""
 
-    def __init__(self, data=None, next_node: 'Node' = None):
+    def __init__(self, data: Any = None, next_node: 'Node' = None):
         """
         Initialize a new node.
         :param data: The data to be stored in the node.
         :param next_node: The next node in the linked structure.
         """
         self._data = data
         self._next = next_node
 
     def __eq__(self, other: 'Node'):
         if isinstance(other, Node):
             return self.data == other.data and self.next == other.next
         return False
 
     @property
-    def data(self):
+    def data(self) -> Any:
         return self._data
 
     @data.setter
-    def data(self, data):
+    def data(self, data: Any) -> None:
         self._data = data
 
     @property
     def next(self) -> 'Node':
         return self._next
 
     @next.setter
-    def next(self, ptr: 'Node'):
+    def next(self, ptr: 'Node') -> None:
         if not isinstance(ptr, (Node, type(None))):
             raise TypeError("The pointer should be a Node or None")
         self._next = ptr
 
 
 class BinaryNode:
     """Node for double side linked data structures"""
-    def __init__(self, data=None, prev_node: 'BinaryNode' = None, next_node: 'BinaryNode' = None):
+    def __init__(self, data: Any = None, prev_node: 'BinaryNode' = None, next_node: 'BinaryNode' = None):
         """
         Initialize a new node.
         :param data: The data to be stored in the node.
         :param prev_node: The previous node
         :param next_node: The next node
         """
         self._data = data
@@ -49,46 +52,46 @@
 
     def __eq__(self, other: 'BinaryNode'):
         if isinstance(other, BinaryNode):
             return self.data == other.data and self.prev == other.prev and self.next == other.next
         return False
 
     @property
-    def data(self):
+    def data(self) -> Any:
         return self._data
 
     @data.setter
-    def data(self, data):
+    def data(self, data: Any) -> None:
         self._data = data
 
     @property
     def prev(self) -> 'BinaryNode':
         return self._prev
 
     @prev.setter
-    def prev(self, ptr: 'BinaryNode'):
+    def prev(self, ptr: 'BinaryNode') -> None:
         if not isinstance(ptr, (BinaryNode, type(None))):
             raise TypeError("The pointer should be a BinaryNode or None")
         self._prev = ptr
 
     @property
     def next(self) -> 'BinaryNode':
         return self._next
 
     @next.setter
-    def next(self, ptr: 'BinaryNode'):
+    def next(self, ptr: 'BinaryNode') -> None:
         if not isinstance(ptr, (BinaryNode, type(None))):
             raise TypeError("The pointer should be a BinaryNode or None")
         self._next = ptr
 
 
 class TreeNode:
     """Node for binary tree based linked data structures"""
 
-    def __init__(self, key=None, left_node: 'TreeNode' = None, right_node: 'TreeNode' = None):
+    def __init__(self, key: Any = None, left_node: 'TreeNode' = None, right_node: 'TreeNode' = None):
         """
         Initialize a new node.
         :param key: The data to be stored in the node.
         :param left_node: The previous node
         :param right_node: The next node
         """
         self._key = key
@@ -97,33 +100,33 @@
 
     def __eq__(self, other: 'TreeNode'):
         if isinstance(other, TreeNode):
             return self.key == other.key and self.left == other.left and self.right == other.right
         return False
 
     @property
-    def key(self):
+    def key(self) -> Any:
         return self._key
 
     @key.setter
-    def key(self, data):
+    def key(self, data: Any) -> None:
         self._key = data
 
     @property
     def left(self) -> 'TreeNode':
         return self._left
 
     @left.setter
-    def left(self, ptr: 'TreeNode'):
+    def left(self, ptr: 'TreeNode') -> None:
         if not isinstance(ptr, (TreeNode, type(None))):
             raise TypeError("The pointer should be a TreeNode or None")
         self._left = ptr
 
     @property
     def right(self) -> 'TreeNode':
         return self._right
 
     @right.setter
-    def right(self, ptr: 'TreeNode'):
+    def right(self, ptr: 'TreeNode') -> None:
         if not isinstance(ptr, (TreeNode, type(None))):
             raise TypeError("The pointer should be a TreeNode or None")
         self._right = ptr
```

### Comparing `PyAlStruct-0.8.0/setup.py` & `pyalstruct-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='PyAlStruct',
-    version='0.8.0',
+    version='0.9.0',
     author='Fathi Abdelmalek',
     author_email='abdelmalek.fathi.2001@gmail.com',
     url='https://github.com/fathiabdelmalek/PyAlStruct',
     description='Implementation of data structures and algorithms in python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['al_struct.algorithms',
```

