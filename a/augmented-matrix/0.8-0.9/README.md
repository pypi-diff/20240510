# Comparing `tmp/augmented_matrix-0.8.tar.gz` & `tmp/augmented_matrix-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augmented_matrix-0.8.tar", last modified: Fri Apr 19 00:17:12 2024, max compression
+gzip compressed data, was "augmented_matrix-0.9.tar", last modified: Wed May  8 19:56:37 2024, max compression
```

## Comparing `augmented_matrix-0.8.tar` & `augmented_matrix-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-19 00:17:12.484227 augmented_matrix-0.8/
--rw-r--r--   0 yumengliu   (501) staff       (20)     1068 2024-04-15 19:47:36.000000 augmented_matrix-0.8/LICENSE
--rw-r--r--   0 yumengliu   (501) staff       (20)     2009 2024-04-19 00:17:12.483937 augmented_matrix-0.8/PKG-INFO
--rw-r--r--   0 yumengliu   (501) staff       (20)      168 2024-04-16 17:23:36.000000 augmented_matrix-0.8/README.md
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-19 00:17:12.482853 augmented_matrix-0.8/augmented_matrix/
--rw-r--r--   0 yumengliu   (501) staff       (20)       32 2024-04-15 23:00:31.000000 augmented_matrix-0.8/augmented_matrix/__init__.py
--rw-r--r--   0 yumengliu   (501) staff       (20)     4949 2024-04-19 00:17:04.000000 augmented_matrix-0.8/augmented_matrix/augmented_matrix.py
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-19 00:17:12.483761 augmented_matrix-0.8/augmented_matrix.egg-info/
--rw-r--r--   0 yumengliu   (501) staff       (20)     2009 2024-04-19 00:17:12.000000 augmented_matrix-0.8/augmented_matrix.egg-info/PKG-INFO
--rw-r--r--   0 yumengliu   (501) staff       (20)      327 2024-04-19 00:17:12.000000 augmented_matrix-0.8/augmented_matrix.egg-info/SOURCES.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)        1 2024-04-19 00:17:12.000000 augmented_matrix-0.8/augmented_matrix.egg-info/dependency_links.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)        6 2024-04-19 00:17:12.000000 augmented_matrix-0.8/augmented_matrix.egg-info/requires.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)       17 2024-04-19 00:17:12.000000 augmented_matrix-0.8/augmented_matrix.egg-info/top_level.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)      613 2024-04-19 00:17:04.000000 augmented_matrix-0.8/pyproject.toml
--rw-r--r--   0 yumengliu   (501) staff       (20)       38 2024-04-19 00:17:12.484272 augmented_matrix-0.8/setup.cfg
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-19 00:17:12.483477 augmented_matrix-0.8/test/
--rw-r--r--   0 yumengliu   (501) staff       (20)     2255 2024-04-16 20:10:05.000000 augmented_matrix-0.8/test/test_augmented_matrix.py
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-05-08 19:56:37.644554 augmented_matrix-0.9/
+-rw-r--r--   0 yumengliu   (501) staff       (20)     1068 2024-04-15 19:47:36.000000 augmented_matrix-0.9/LICENSE
+-rw-r--r--   0 yumengliu   (501) staff       (20)     2009 2024-05-08 19:56:37.644371 augmented_matrix-0.9/PKG-INFO
+-rw-r--r--   0 yumengliu   (501) staff       (20)      168 2024-04-16 17:23:36.000000 augmented_matrix-0.9/README.md
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-05-08 19:56:37.642817 augmented_matrix-0.9/augmented_matrix/
+-rw-r--r--   0 yumengliu   (501) staff       (20)       32 2024-04-15 23:00:31.000000 augmented_matrix-0.9/augmented_matrix/__init__.py
+-rw-r--r--   0 yumengliu   (501) staff       (20)     6001 2024-05-08 19:53:04.000000 augmented_matrix-0.9/augmented_matrix/augmented_matrix.py
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-05-08 19:56:37.644189 augmented_matrix-0.9/augmented_matrix.egg-info/
+-rw-r--r--   0 yumengliu   (501) staff       (20)     2009 2024-05-08 19:56:37.000000 augmented_matrix-0.9/augmented_matrix.egg-info/PKG-INFO
+-rw-r--r--   0 yumengliu   (501) staff       (20)      327 2024-05-08 19:56:37.000000 augmented_matrix-0.9/augmented_matrix.egg-info/SOURCES.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)        1 2024-05-08 19:56:37.000000 augmented_matrix-0.9/augmented_matrix.egg-info/dependency_links.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)        6 2024-05-08 19:56:37.000000 augmented_matrix-0.9/augmented_matrix.egg-info/requires.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)       17 2024-05-08 19:56:37.000000 augmented_matrix-0.9/augmented_matrix.egg-info/top_level.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)      613 2024-05-08 19:56:03.000000 augmented_matrix-0.9/pyproject.toml
+-rw-r--r--   0 yumengliu   (501) staff       (20)       38 2024-05-08 19:56:37.644588 augmented_matrix-0.9/setup.cfg
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-05-08 19:56:37.643910 augmented_matrix-0.9/test/
+-rw-r--r--   0 yumengliu   (501) staff       (20)     2856 2024-05-08 19:53:04.000000 augmented_matrix-0.9/test/test_augmented_matrix.py
```

### Comparing `augmented_matrix-0.8/LICENSE` & `augmented_matrix-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `augmented_matrix-0.8/PKG-INFO` & `augmented_matrix-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augmented-matrix
-Version: 0.8
+Version: 0.9
 Summary: A package that solves augmented matrices into reduced echelon forms
 Author-email: Yumeng Liu <lym20041026@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `augmented_matrix-0.8/augmented_matrix/augmented_matrix.py` & `augmented_matrix-0.9/augmented_matrix/augmented_matrix.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy
 import numpy as np
 from fractions import Fraction
 
 
 class NoSolutionError(Exception):
     pass
 
@@ -14,14 +15,17 @@
 
         self._matrix = np.asarray([[Fraction(j).limit_denominator() for j in i] for i in matrix], **kwargs)
 
         if constraint is not None:
             constraint = np.asarray([Fraction(i).limit_denominator() for i in constraint], **kwargs)
             self._matrix = np.append(self._matrix, [[i] for i in constraint], axis=1)
 
+        self._swap_factor = 1
+        self._mult_factor = 1
+
     @property
     def matrix(self) -> np.ndarray:
         """
         :return: the augmented matrix
         """
         return self._matrix
 
@@ -67,24 +71,27 @@
         while row < (row_count := matrix.shape[0]) and column < matrix.shape[1]:
             # Use the highest absolute value as pivot
             max_row_index = row
             for i in range(row, matrix.shape[0]):
                 if abs(matrix[i][column]) > abs(matrix[max_row_index][column]):
                     max_row_index = i
 
-            matrix[[row, max_row_index]] = matrix[[max_row_index, row]]
+            if row != max_row_index:
+                matrix[[row, max_row_index]] = matrix[[max_row_index, row]]
+                self._swap_factor *= -1
 
             pivot = matrix[row][column]
             if pivot != 0:
                 for i in range(row + 1, row_count):
                     leading_value = matrix[i][column]
                     if leading_value == 0:
                         continue
                     factor = -1 * pivot / leading_value
                     matrix[i] = factor * matrix[i] + matrix[row]
+                    self._mult_factor *= factor
 
             column += 1
             row = column
 
         self._matrix = matrix
         return matrix
 
@@ -109,15 +116,14 @@
         """
         Transforms the matrix from upper triangular form to reduced echelon form
         :raise: NoSolutionException: if the matrix has no solution
         """
         if not self.check_upper_triangular():
             self.partial_pivot()
 
-        self.check_valid_solution()
         self.simplify_echelon()
 
         matrix = self._matrix
         for row_index in range(matrix.shape[0] - 1, -1, -1):
             pivot_coord = None
             for element_index in range(matrix.shape[1] - 1):
                 if matrix[row_index][element_index] != 0:
@@ -135,19 +141,42 @@
                     pivot = matrix[pivot_coord[0]][pivot_coord[1]]
                     factor = -1 * leading / pivot
                     matrix[i] = factor * matrix[pivot_coord[0]] + matrix[i]
 
         self._matrix = matrix
         return matrix
 
-    def solve(self) -> np.ndarray:
+    def solve(self, return_type=float) -> np.ndarray:
         """
         Solves the augmented matrix
         :returns self._matrix: the row-reduced matrix
         :raises NoSolutionException: if the matrix has no solution
         """
         self.partial_pivot()
         self.reduce_echelon()
-        return self._matrix
+        self.check_valid_solution()
+        return self._matrix.astype(return_type)
+
+    def is_square(self) -> bool:
+        """
+        Checks if the matrix is square (the dimensions are equal and the matrix is 2D)
+        :returns True: if the matrix is square
+        :returns False: if the matrix is not square
+        """
+        shape = self._matrix.shape
+        return len(shape) == 2 and shape[0] == shape[1]
+
+    def determinant(self):
+        """
+        Calculates the determinant of the matrix
+        :return: a value indicating the determinant of this matrix
+        :raises NoSolutionException: if the matrix is not square
+        """
+
+        if self.is_square():
+            self.partial_pivot()
+            return numpy.prod(self._matrix.diagonal(), axis=0) * self._swap_factor / self._mult_factor
+        else:
+            raise NoSolutionError("The matrix is not square")
 
 
 __all__ = ['AugmentedMatrix', 'NoSolutionError']
```

### Comparing `augmented_matrix-0.8/augmented_matrix.egg-info/PKG-INFO` & `augmented_matrix-0.9/augmented_matrix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augmented-matrix
-Version: 0.8
+Version: 0.9
 Summary: A package that solves augmented matrices into reduced echelon forms
 Author-email: Yumeng Liu <lym20041026@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `augmented_matrix-0.8/pyproject.toml` & `augmented_matrix-0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "augmented-matrix"
-version = "0.8"
+version = "0.9"
 authors = [
   { name="Yumeng Liu", email="lym20041026@gmail.com" }
 ]
 description = "A package that solves augmented matrices into reduced echelon forms"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies= ['numpy']
```

### Comparing `augmented_matrix-0.8/test/test_augmented_matrix.py` & `augmented_matrix-0.9/test/test_augmented_matrix.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,34 +3,38 @@
 from fractions import Fraction
 
 
 class TestAugmentedMatrix(unittest.TestCase):
     def _to_fraction(self, original):
         return [[Fraction(j).limit_denominator() for j in i] for i in original]
 
-    def check_solution_equal(self, unsolved, expected, constraint=None):
+    def check_matrix_equal(self, unsolved, expected, constraint=None):
         if constraint is not None:
             constraint = [Fraction(j).limit_denominator() for j in constraint]
         m = AugmentedMatrix(self._to_fraction(unsolved), constraint)
         m.solve()
         self.assertEqual(m.matrix.tolist(), self._to_fraction(expected))
 
+    def check_determinant(self, matrix, expected_determinant):
+        m = AugmentedMatrix(matrix)
+        self.assertEqual(m.determinant(), expected_determinant)
+
     def test_augmented_matrix(self):
         original_matrix = [
             [3, 5, -1, 10],
             [1, 4, 1, 7],
             [9, 0, 2, 1]
         ]
 
         expected = [
             [1, 0, 0, 0.2],
             [0, 1, 0, 1.8],
             [0, 0, 1, -0.4]
         ]
-        self.check_solution_equal(original_matrix, expected)
+        self.check_matrix_equal(original_matrix, expected)
 
     def test_call_reduce_echelon_when_non_echelon(self):
         m = AugmentedMatrix(self._to_fraction([
             [1, 2, 3, 4],
             [0, 1, 2, 2],
             [0, 1, 1, 3]
         ]))
@@ -44,37 +48,54 @@
 
     def test_augmented_matrix_no_solution(self):
         original = [
             [1, 2, 3],
             [1, 2, 4]
         ]
         with self.assertRaises(NoSolutionError):
-            self.check_solution_equal(original, [])
+            self.check_matrix_equal(original, [])
 
     def test_augmented_matrix_with_free_variable(self):
         original_matrix = [
             [1, 2, 3],
             [2, 4, 6]
         ]
         expected = [
             [1, 2, 3],
             [0, 0, 0]
         ]
-        self.check_solution_equal(original_matrix, expected)
+        self.check_matrix_equal(original_matrix, expected)
 
     def test_augmented_matrix_with_constraint(self):
         original_matrix = [
             [3, 5, -1],
             [1, 4, 1],
             [9, 0, 2]
         ]
         constraint = [10, 7, 1]
         expected = [
             [1, 0, 0, 0.2],
             [0, 1, 0, 1.8],
             [0, 0, 1, -0.4]
         ]
-        self.check_solution_equal(original_matrix, expected, constraint=constraint)
+        self.check_matrix_equal(original_matrix, expected, constraint=constraint)
+
+    def test_determinant(self):
+        matrix = [
+            [2, -8, 6, 8],
+            [3, -9, 5, 10],
+            [-3, 0, 1, -2],
+            [1, -4, 0, 6]
+        ]
+        self.check_determinant(matrix, -36)
+
+    def test_non_square_matrix_determinant_raise_error(self):
+        matrix = [
+            [1, 2, 3],
+            [4, 5, 6]
+        ]
+        with self.assertRaises(NoSolutionError):
+            self.check_determinant(matrix, 1)
 
 
 if __name__ == '__main__':
     unittest.main()
```

