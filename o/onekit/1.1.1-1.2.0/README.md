# Comparing `tmp/onekit-1.1.1.tar.gz` & `tmp/onekit-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onekit-1.1.1.tar", max compression
+gzip compressed data, was "onekit-1.2.0.tar", max compression
```

## Comparing `onekit-1.1.1.tar` & `onekit-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1514 2024-05-06 21:25:32.769600 onekit-1.1.1/LICENSE
--rw-r--r--   0        0        0     1569 2024-05-06 21:25:32.769600 onekit-1.1.1/README.md
--rw-r--r--   0        0        0     2217 2024-05-06 21:26:27.089794 onekit-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       88 2024-05-06 21:25:32.809601 onekit-1.1.1/src/onekit/__init__.py
--rw-r--r--   0        0        0     3965 2024-05-06 21:25:32.809601 onekit-1.1.1/src/onekit/mathkit.py
--rw-r--r--   0        0        0     1643 2024-05-06 21:25:32.809601 onekit-1.1.1/src/onekit/numpykit.py
--rw-r--r--   0        0        0    14598 2024-05-06 21:25:32.809601 onekit-1.1.1/src/onekit/optfunckit.py
--rw-r--r--   0        0        0     6799 2024-05-06 21:25:32.809601 onekit-1.1.1/src/onekit/pandaskit.py
--rw-r--r--   0        0        0    37190 2024-05-06 21:25:32.809601 onekit-1.1.1/src/onekit/pythonkit.py
--rw-r--r--   0        0        0    38022 2024-05-06 21:25:32.809601 onekit-1.1.1/src/onekit/sparkkit.py
--rw-r--r--   0        0        0    19542 2024-05-06 21:25:32.809601 onekit-1.1.1/src/onekit/vizkit.py
--rw-r--r--   0        0        0     2483 1970-01-01 00:00:00.000000 onekit-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1514 2024-05-10 11:14:38.092935 onekit-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1569 2024-05-10 11:14:38.092935 onekit-1.2.0/README.md
+-rw-r--r--   0        0        0     2254 2024-05-10 11:15:25.592680 onekit-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2024-05-10 11:14:38.132935 onekit-1.2.0/src/onekit/__init__.py
+-rw-r--r--   0        0        0     6032 2024-05-10 11:14:38.132935 onekit-1.2.0/src/onekit/mathkit.py
+-rw-r--r--   0        0        0     2155 2024-05-10 11:14:38.132935 onekit-1.2.0/src/onekit/numpykit.py
+-rw-r--r--   0        0        0    14598 2024-05-10 11:14:38.132935 onekit-1.2.0/src/onekit/optfunckit.py
+-rw-r--r--   0        0        0     6799 2024-05-10 11:14:38.132935 onekit-1.2.0/src/onekit/pandaskit.py
+-rw-r--r--   0        0        0    37190 2024-05-10 11:14:38.132935 onekit-1.2.0/src/onekit/pythonkit.py
+-rw-r--r--   0        0        0    39391 2024-05-10 11:14:38.136935 onekit-1.2.0/src/onekit/sparkkit.py
+-rw-r--r--   0        0        0    19542 2024-05-10 11:14:38.136935 onekit-1.2.0/src/onekit/vizkit.py
+-rw-r--r--   0        0        0     2483 1970-01-01 00:00:00.000000 onekit-1.2.0/PKG-INFO
```

### Comparing `onekit-1.1.1/LICENSE` & `onekit-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onekit-1.1.1/README.md` & `onekit-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `onekit-1.1.1/pyproject.toml` & `onekit-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onekit"
-version = "1.1.1"
+version = "1.2.0"
 description = "All-in-One Python Kit."
 authors = ["Eugen Stripling <estripling042@gmail.com>"]
 license = "BSD 3-Clause"
 readme = "README.md"
 repository = "https://github.com/estripling/onekit"
 documentation = "https://onekit.readthedocs.io/en/stable/"
 keywords = ["onekit"]
@@ -30,23 +30,23 @@
 pre-commit = "^3.5.0"
 pre-commit-hooks = "^4.5.0"
 
 [tool.poetry.group.testing.dependencies]
 pytest = "^7.4.3"
 pytest-cov = "^4.1.0"
 pytest-skip-slow = "^0.0.5"
+time-machine = "^2.13.0"
 
 [tool.poetry.group.docs.dependencies]
 furo = "^2023.9.10"
 jupyterlab = "^4.0.8"
 myst-parser = "^2.0.0"
 nbsphinx = "^0.9.3"
 sphinx-autoapi = "^3.0.0"
 sphinx-copybutton = "^0.5.2"
-time-machine = "^2.13.0"
 
 [tool.poetry.group.packaging.dependencies]
 python-semantic-release = "^8.3.0"
 
 [tool.poetry.group.pandaskit.dependencies]
 pandas = ">=0.23.2"
 
@@ -70,15 +70,18 @@
 multi_line_output = 3
 
 [tool.pytest.ini_options]
 markers = [
     "slow: marks tests as slow (deselect with '-m \"not slow\"')",
     "serial",
 ]
-filterwarnings = ["ignore::DeprecationWarning"]
+filterwarnings = [
+    "ignore::DeprecationWarning",
+    "ignore::RuntimeWarning",
+]
 
 [tool.semantic_release]
 branch = "main"
 version_variables = ["pyproject.toml:version"]
 changelog_file = "CHANGELOG.md"
 build_command = "poetry build"
 dist_path = "dist/"
```

### Comparing `onekit-1.1.1/src/onekit/mathkit.py` & `onekit-1.2.0/src/onekit/mathkit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+import math
 from typing import (
     Generator,
     Union,
 )
 
 import toolz
 
 __all__ = (
     "collatz",
+    "digitscale",
     "fibonacci",
     "isdivisible",
     "iseven",
     "isodd",
+    "sign",
 )
 
 
 def collatz(n: int, /) -> Generator:
     """Generate a Collatz sequence.
 
     The famous 3n + 1 conjecture [c1]_ [c2]_. Given a positive integer :math:`n > 0`,
@@ -75,14 +78,57 @@
         if n == 1:
             break
 
         # update
         n = n // 2 if iseven(n) else 3 * n + 1
 
 
+def digitscale(x: Union[int, float], /) -> float:
+    """Scale :math:`x` such that its mapped integer part is its number of digits.
+
+    Given a number :math:`x \\in \\mathbb{R}`, the following function
+    :math:`f \\colon \\mathbb{R} \\rightarrow \\mathbb{R}_{\\ge 0}` scales it such that
+    its mapped integer part :math:`\\lfloor f(x) \\rfloor \\in \\mathbb{N}_{0}`
+    is the number of digits in :math:`[x]`:
+
+    .. math::
+
+        f(x) =
+        \\begin{cases}
+            1 + \\log_{10}|x| & \\text{ if } |x| \\ge 0.1 \\\\[6pt]
+            0 & \\text{ otherwise }
+        \\end{cases}
+
+    Notes
+    -----
+    - :math:`\\lfloor \\cdot \\rfloor`: floor function
+    - :math:`\\left[ \\, \\cdot \\, \\right]`: truncation function
+    - For any positive integer :math:`n`, the number of digits in :math:`n` is
+      :math:`1 + \\lfloor \\log_{10} n \\rfloor`
+
+    See Also
+    --------
+    onekit.numpykit.digitscale : NumPy version
+    onekit.sparkkit.with_digitscale : PySpark version
+
+    Examples
+    --------
+    >>> import onekit.mathkit as mk
+    >>> list(map(mk.digitscale, [0.1, 1, 10, 100, 1_000, 10_000, 100_000, 1_000_000]))
+    [0.0, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0]
+
+    >>> list(map(mk.digitscale, [0.2, 2, 20, 200]))
+    [0.30102999566398125, 1.3010299956639813, 2.3010299956639813, 3.3010299956639813]
+
+    >>> list(map(mk.digitscale, [-0.5, -5, -50, -500]))
+    [0.6989700043360187, 1.6989700043360187, 2.6989700043360187, 3.6989700043360187]
+    """
+    return 1 + math.log10(abs(x)) if abs(x) >= 0.1 else 0.0
+
+
 def fibonacci() -> Generator:
     """Generate the Fibonacci sequence.
 
     For :math:`n > 1`, Fibonacci numbers may be defined by [f1]_ [f2]_:
 
     .. math::
 
@@ -178,7 +224,34 @@
     >>> mk.isodd(1)
     True
 
     >>> mk.isodd(2)
     False
     """
     return toolz.complement(iseven)(x)
+
+
+def sign(x: Union[int, float], /) -> int:
+    """Sign function.
+
+    .. math::
+
+        f(x) =
+        \\begin{cases}
+            -1 & \\text{ if } x < 0 \\\\[6pt]
+            0 & \\text{ if } x = 0 \\\\[6pt]
+            1 & \\text{ if } x > 0
+        \\end{cases}
+
+    Examples
+    --------
+    >>> import onekit.mathkit as mk
+    >>> mk.sign(0)
+    0
+
+    >>> mk.sign(3.14)
+    1
+
+    >>> mk.sign(-10)
+    -1
+    """
+    return int(0 if math.isclose(x, 0) else math.copysign(1, x))
```

### Comparing `onekit-1.1.1/src/onekit/numpykit.py` & `onekit-1.2.0/src/onekit/numpykit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import numpy as np
 import numpy.typing as npt
 
+import onekit.mathkit as mk
+
 __all__ = (
     "check_vector",
+    "digitscale",
     "stderr",
 )
 
 
 ArrayLike = npt.ArrayLike
 Vector = npt.NDArray[np.float64]
 
@@ -45,14 +48,31 @@
         domain = f"[{n_min}, {n_max}"
         domain = f"{domain}]" if np.isfinite(n_max) else f"{domain})"
         raise TypeError(f"x with n={len(x)} - n must be an integer in {domain}")
 
     return x
 
 
+def digitscale(x: ArrayLike, /) -> np.ndarray:
+    """NumPy version of digitscale.
+
+    See Also
+    --------
+    onekit.mathkit.digitscale : Python version
+    onekit.sparkkit.with_digitscale : PySpark version
+
+    Examples
+    --------
+    >>> import onekit.numpykit as npk
+    >>> npk.digitscale([0.1, 1, 10, 100, 1_000, 10_000, 100_000, 1_000_000])
+    array([0., 1., 2., 3., 4., 5., 6., 7.])
+    """
+    return np.vectorize(mk.digitscale, otypes=[float])(x)
+
+
 def stderr(x: ArrayLike, /) -> float:
     """Compute standard error of the mean.
 
     Examples
     --------
     >>> import numpy as np
     >>> import onekit.numpykit as npk
```

### Comparing `onekit-1.1.1/src/onekit/optfunckit.py` & `onekit-1.2.0/src/onekit/optfunckit.py`

 * *Files identical despite different names*

### Comparing `onekit-1.1.1/src/onekit/pandaskit.py` & `onekit-1.2.0/src/onekit/pandaskit.py`

 * *Files identical despite different names*

### Comparing `onekit-1.1.1/src/onekit/pythonkit.py` & `onekit-1.2.0/src/onekit/pythonkit.py`

 * *Files identical despite different names*

### Comparing `onekit-1.1.1/src/onekit/sparkkit.py` & `onekit-1.2.0/src/onekit/sparkkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     "is_schema_equal",
     "join",
     "peek",
     "str_to_col",
     "union",
     "with_date_diff_ago",
     "with_date_diff_ahead",
+    "with_digitscale",
     "with_endofweek_date",
     "with_increasing_id",
     "with_index",
     "with_startofweek_date",
     "with_weekday",
 )
 
@@ -1140,14 +1141,67 @@
 
     def inner(df: SparkDF, /) -> SparkDF:
         return df.withColumn(new_col, F.datediff(str_to_col(date_col), F.lit(d0)))
 
     return inner
 
 
+def with_digitscale(num_col: str, new_col: str) -> SparkDFTransformFunc:
+    """PySpark version of digitscale.
+
+    See Also
+    --------
+    onekit.mathkit.digitscale : Python version
+    onekit.numpykit.digitscale : NumPy version
+
+    Examples
+    --------
+    >>> from pyspark.sql import SparkSession
+    >>> import onekit.sparkkit as sk
+    >>> spark = SparkSession.builder.getOrCreate()
+    >>> df = spark.createDataFrame(
+    ...     [
+    ...         dict(x=0.1),
+    ...         dict(x=1.0),
+    ...         dict(x=10.0),
+    ...         dict(x=100.0),
+    ...         dict(x=1_000.0),
+    ...         dict(x=10_000.0),
+    ...         dict(x=100_000.0),
+    ...         dict(x=1_000_000.0),
+    ...         dict(x=None),
+    ...     ],
+    ... )
+    >>> df.transform(sk.with_digitscale("x", "fx")).show()
+    +---------+----+
+    |        x|  fx|
+    +---------+----+
+    |      0.1| 0.0|
+    |      1.0| 1.0|
+    |     10.0| 2.0|
+    |    100.0| 3.0|
+    |   1000.0| 4.0|
+    |  10000.0| 5.0|
+    | 100000.0| 6.0|
+    |1000000.0| 7.0|
+    |     null|null|
+    +---------+----+
+    <BLANKLINE>
+    """
+
+    def inner(df: SparkDF, /) -> SparkDF:
+        x = F.abs(num_col)
+        return df.withColumn(
+            new_col,
+            F.when(x.isNull(), None).when(x >= 0.1, 1 + F.log10(x)).otherwise(0.0),
+        )
+
+    return inner
+
+
 def with_endofweek_date(
     date_col: str,
     new_col: str,
     last_weekday: str = "Sun",
 ) -> SparkDFTransformFunc:
     """Add column with the end of the week date.
```

### Comparing `onekit-1.1.1/src/onekit/vizkit.py` & `onekit-1.2.0/src/onekit/vizkit.py`

 * *Files identical despite different names*

### Comparing `onekit-1.1.1/PKG-INFO` & `onekit-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onekit
-Version: 1.1.1
+Version: 1.2.0
 Summary: All-in-One Python Kit.
 Home-page: https://github.com/estripling/onekit
 License: BSD 3-Clause
 Keywords: onekit
 Author: Eugen Stripling
 Author-email: estripling042@gmail.com
 Requires-Python: >=3.8.1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onekit Version: 1.1.1 Summary: All-in-One Python
+Metadata-Version: 2.1 Name: onekit Version: 1.2.0 Summary: All-in-One Python
 Kit. Home-page: https://github.com/estripling/onekit License: BSD 3-Clause
 Keywords: onekit Author: Eugen Stripling Author-email: estripling042@gmail.com
 Requires-Python: >=3.8.1 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
```

