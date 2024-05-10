# Comparing `tmp/lapx-0.5.8.tar.gz` & `tmp/lapx-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapx-0.5.8.tar", last modified: Mon Apr 29 23:23:20 2024, max compression
+gzip compressed data, was "lapx-0.5.9.tar", last modified: Fri May 10 16:48:55 2024, max compression
```

## Comparing `lapx-0.5.8.tar` & `lapx-0.5.9.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:23:20.365656 lapx-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-29 23:23:09.000000 lapx-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-29 23:23:09.000000 lapx-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-29 23:23:20.365656 lapx-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-29 23:23:09.000000 lapx-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:23:20.357656 lapx-0.5.8/_lapjv_src/
--rw-r--r--   0 runner    (1001) docker     (127)   569034 2024-04-29 23:23:20.000000 lapx-0.5.8/_lapjv_src/_lapjv.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-29 23:23:09.000000 lapx-0.5.8/_lapjv_src/_lapjv.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     8763 2024-04-29 23:23:09.000000 lapx-0.5.8/_lapjv_src/lapjv.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-29 23:23:09.000000 lapx-0.5.8/_lapjv_src/lapjv.h
--rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-04-29 23:23:09.000000 lapx-0.5.8/_lapjv_src/lapmod.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:23:20.361656 lapx-0.5.8/lap/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-29 23:23:09.000000 lapx-0.5.8/lap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-29 23:23:09.000000 lapx-0.5.8/lap/lapmod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:23:20.361656 lapx-0.5.8/lap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 23:23:09.000000 lapx-0.5.8/lap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1415310 2024-04-29 23:23:09.000000 lapx-0.5.8/lap/tests/cost_eps.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-29 23:23:09.000000 lapx-0.5.8/lap/tests/test_arr_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-04-29 23:23:09.000000 lapx-0.5.8/lap/tests/test_lapjv.py
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-29 23:23:09.000000 lapx-0.5.8/lap/tests/test_lapmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-29 23:23:09.000000 lapx-0.5.8/lap/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:23:20.361656 lapx-0.5.8/lapx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-29 23:23:20.000000 lapx-0.5.8/lapx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-29 23:23:20.000000 lapx-0.5.8/lapx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 23:23:20.000000 lapx-0.5.8/lapx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-29 23:23:20.000000 lapx-0.5.8/lapx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-29 23:23:20.000000 lapx-0.5.8/lapx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-29 23:23:09.000000 lapx-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-29 23:23:09.000000 lapx-0.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 23:23:20.365656 lapx-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-29 23:23:09.000000 lapx-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:48:55.054709 lapx-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-10 16:48:45.000000 lapx-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-10 16:48:45.000000 lapx-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-10 16:48:55.054709 lapx-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-10 16:48:45.000000 lapx-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:48:55.050709 lapx-0.5.9/_lapjv_src/
+-rw-r--r--   0 runner    (1001) docker     (127)   569130 2024-05-10 16:48:54.000000 lapx-0.5.9/_lapjv_src/_lapjv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-05-10 16:48:45.000000 lapx-0.5.9/_lapjv_src/_lapjv.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     8763 2024-05-10 16:48:45.000000 lapx-0.5.9/_lapjv_src/lapjv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-10 16:48:45.000000 lapx-0.5.9/_lapjv_src/lapjv.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-05-10 16:48:45.000000 lapx-0.5.9/_lapjv_src/lapmod.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:48:55.050709 lapx-0.5.9/lap/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-10 16:48:45.000000 lapx-0.5.9/lap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-10 16:48:45.000000 lapx-0.5.9/lap/lapmod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:48:55.054709 lapx-0.5.9/lap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 16:48:45.000000 lapx-0.5.9/lap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1415310 2024-05-10 16:48:45.000000 lapx-0.5.9/lap/tests/cost_eps.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-10 16:48:45.000000 lapx-0.5.9/lap/tests/test_arr_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-05-10 16:48:45.000000 lapx-0.5.9/lap/tests/test_lapjv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-05-10 16:48:45.000000 lapx-0.5.9/lap/tests/test_lapmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-10 16:48:45.000000 lapx-0.5.9/lap/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:48:55.054709 lapx-0.5.9/lapx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-10 16:48:55.000000 lapx-0.5.9/lapx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-10 16:48:55.000000 lapx-0.5.9/lapx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 16:48:55.000000 lapx-0.5.9/lapx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 16:48:55.000000 lapx-0.5.9/lapx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-10 16:48:55.000000 lapx-0.5.9/lapx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-10 16:48:45.000000 lapx-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 16:48:55.054709 lapx-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-10 16:48:45.000000 lapx-0.5.9/setup.py
```

### Comparing `lapx-0.5.8/LICENSE` & `lapx-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lapx-0.5.8/PKG-INFO` & `lapx-0.5.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lapx
-Version: 0.5.8
+Version: 0.5.9
 Summary: Linear Assignment Problem solver (LAPJV/LAPMOD).
 Home-page: https://github.com/rathaROG/lapx
 Author: rathaROG
 License: BSD-2-Clause
 Keywords: Linear Assignment,LAPJV,LAPMOD,lap
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -28,124 +28,97 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Cython>=0.29.32
 Requires-Dist: numpy>=1.21.6
 
 [![Test Simple](https://github.com/rathaROG/lapx/actions/workflows/test_simple.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/test_simple.yaml)
 [![Benchmark](https://github.com/rathaROG/lapx/actions/workflows/benchmark.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/benchmark.yaml)
 [![Test PyPI Build](https://github.com/rathaROG/lapx/actions/workflows/prepublish.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/prepublish.yaml)
 [![Publish to PyPI](https://github.com/rathaROG/lapx/actions/workflows/publish.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/publish.yaml)
 
 # Linear Assignment Problem Solver
 
-`lapx` basically is Tomas Kazmar's [`gatagat/lap`](https://github.com/gatagat/lap) with support for all Windows/Linux/macOS and Python 3.7/3.8/3.9/3.10/3.11/3.12.
+`lapx` basically is Tomas Kazmar's [`gatagat/lap`](https://github.com/gatagat/lap) with support for all Windows/Linux/macOS and Python 3.7-3.12. 
 
-* Based on: [[ed04ab7752]](https://github.com/gatagat/lap/tree/ed04ab7752c7c9688ddcbae534633f34ce04361f)
-* License: BSD-2-Clause, see [`LICENSE`](LICENSE) @[`gatagat`](https://github.com/gatagat)
+## 💽 Installation
 
-## 💽 Installation:
+### Install from [PyPI](https://pypi.org/project/lapx/):
 
-* Install from [PyPI](https://pypi.org/project/lapx/):
+[![PyPI version](https://badge.fury.io/py/lapx.svg)](https://badge.fury.io/py/lapx)
+[![Downloads](https://static.pepy.tech/badge/lapx)](https://pepy.tech/project/lapx)
+[![Downloads](https://static.pepy.tech/badge/lapx/month)](https://pepy.tech/project/lapx)
 
-  ```
-  pip install lapx
-  ```
-
-  | **Pre-built Wheels** 🛞 | **Windows** ✅ | **Linux** ✅ | **macOS** ✅ |
-  |:---:|:---:|:---:|:---:|
-  | Python v3.7 | AMD64 | x86_64/aarch64 ² | x86_64 |
-  | Python v3.8 | AMD64 | x86_64/aarch64 ² | x86_64/arm64 |
-  | Python v3.9 | AMD64/ARM64 ¹ | x86_64/aarch64 ² | x86_64/arm64 |
-  | Python v3.10 | AMD64/ARM64 ¹ | x86_64/aarch64 ² | x86_64/arm64 |
-  | Python v3.11 | AMD64/ARM64 ¹ | x86_64/aarch64 ² | x86_64/arm64 |
-  | Python v3.12 | AMD64/ARM64 ¹ | x86_64/aarch64 ² | x86_64/arm64 |
-
-  <sup>¹ Windows ARM64 is experimental.</sup><br>
-  <sup>² Linux now includes both `manylinux` and `musllinux`.</sup><br>
-
-* Or install from GitHub repo directly (Require C++ compiler):
-
-  ```
-  pip install git+https://github.com/rathaROG/lapx.git
-  ```
-
-* Or clone and build on your local machine (Require C++ compiler):
+```
+pip install lapx
+```
 
-  <details><summary><ins>Click here to expand!</ins></summary>
-  
-  ```
-  git clone https://github.com/rathaROG/lapx.git
-  cd lapx
-  python -m pip install --upgrade pip
-  pip install "setuptools>=67.2.0"
-  pip install wheel build
-  python -m build --wheel
-  cd dist
-  ```
-  
-  </details>
+| **Pre-built Wheels** 🛞 | **Windows** ✅ | **Linux** ✅ | **macOS** ✅ |
+|:---:|:---:|:---:|:---:|
+| Python 3.7 | AMD64 | x86_64/aarch64 | x86_64 |
+| Python 3.8 | AMD64 | x86_64/aarch64 | x86_64/arm64 |
+| Python 3.9-3.12 | AMD64/ARM64 ¹ | x86_64/aarch64 | x86_64/arm64 |
 
-## 🧪 Usage:
+<sup>¹ Windows ARM64 is experimental.</sup><br>
 
-* `lapx` is just the name for package distribution.
-* The same as `lap`, use `import lap` to import; for example:
+<details><summary>Click here to expand!</summary>
 
-  ```
-  import lap
-  import numpy as np
-  print(lap.lapjv(np.random.rand(4, 5), extend_cost=True))
-  ```
+### Install from GitHub repo (Require C++ compiler):
 
-<br />
+```
+pip install git+https://github.com/rathaROG/lapx.git
+```
 
-<details><summary>Click here to show more...</summary>
+### Build and install (Require C++ compiler):
 
-<br />
+```
+git clone https://github.com/rathaROG/lapx.git
+cd lapx
+pip install "setuptools>=67.8.0"
+pip install wheel build
+python -m build --wheel
+cd dist
+```
 
-lap: Linear Assignment Problem solver
-=====================================
+</details>
 
-**lap** is a [linear assignment
-problem](https://en.wikipedia.org/wiki/Assignment_problem) solver using
-Jonker-Volgenant algorithm for dense (LAPJV [1]) or sparse (LAPMOD [2])
-matrices.
+## 🧪 Usage
 
-Both algorithms are implemented from scratch based solely on the papers [1,2]
-and the public domain Pascal implementation provided by A. Volgenant [3].
+`lapx` is just the name for package distribution. The same as `lap`, use `import lap` to import; for example:
 
-In my tests the LAPMOD implementation seems to be faster than the LAPJV
-implementation for matrices with a side of more than ~5000 and with less than
-50% finite coefficients.
+```
+import lap
+import numpy as np
+print(lap.lapjv(np.random.rand(4, 5), extend_cost=True))
+```
 
-[1] R. Jonker and A. Volgenant, "A Shortest Augmenting Path Algorithm for Dense
-and Sparse Linear Assignment Problems", Computing 38, 325-340 (1987)<br>
-[2] A. Volgenant, "Linear and Semi-Assignment Problems: A Core Oriented
-Approach", Computer Ops Res. 23, 917-932 (1996)<br>
-[3] http://www.assignmentproblems.com/LAPJV.htm
+## 🔎 More about LAP
 
+<details><summary>Click here to expand!</summary><br>
 
-### Usage
+Tomas Kazmar's [`gatagat/lap`](https://github.com/gatagat/lap) is a [linear assignment problem](https://en.wikipedia.org/wiki/Assignment_problem) solver using Jonker-Volgenant algorithm for dense LAPJV ¹ or sparse LAPMOD ² matrices. Both algorithms are implemented from scratch based solely on the papers ¹˒² and the public domain Pascal implementation provided by A. Volgenant ³. The LAPMOD implementation seems to be faster than the LAPJV implementation for matrices with a side of more than ~5000 and with less than 50% finite coefficients.
 
-```
-cost, x, y = lap.lapjv(C)
-```
+<sup>¹ R. Jonker and A. Volgenant, "A Shortest Augmenting Path Algorithm for Dense and Sparse Linear Assignment Problems", Computing 38, 325-340 (1987) </sup><br>
+<sup>² A. Volgenant, "Linear and Semi-Assignment Problems: A Core Oriented Approach", Computer Ops Res. 23, 917-932 (1996) </sup><br>
+<sup>³ http://www.assignmentproblems.com/LAPJV.htm </sup><br>
+  
+### `cost, x, y = lap.lapjv(C)`
 
-The function `lapjv(C)` returns the assignment cost (`cost`) and two arrays, `x, y`. If cost matrix `C` has shape N x M, then `x` is a size-N array specifying to which column is row is assigned, and `y` is a size-M array specifying to which row each column is assigned. For example, an output of `x = [1, 0]` indicates that row 0 is assigned to column 1 and row 1 is assigned to column 0. Similarly, an output of `x = [2, 1, 0]` indicates that row 0 is assigned to column 2, row 1 is assigned to column 1, and row 2 is assigned to column 0.
+The function `lapjv(C)` returns the assignment cost `cost` and two arrays `x` and `y`. If cost matrix `C` has shape NxM, then `x` is a size-N array specifying to which column is row is assigned, and `y` is a size-M array specifying to which row each column is assigned. For example, an output of `x = [1, 0]` indicates that row 0 is assigned to column 1 and row 1 is assigned to column 0. Similarly, an output of `x = [2, 1, 0]` indicates that row 0 is assigned to column 2, row 1 is assigned to column 1, and row 2 is assigned to column 0.
 
 Note that this function *does not* return the assignment matrix (as done by scipy's [`linear_sum_assignment`](https://docs.scipy.org/doc/scipy-0.18.1/reference/generated/scipy.optimize.linear_sum_assignment.html) and lapsolver's [`solve dense`](https://github.com/cheind/py-lapsolver)). The assignment matrix can be constructed from `x` as follows:
 ```
 A = np.zeros((N, M))
 for i in range(N):
     A[i, x[i]] = 1
 ```
+
 Equivalently, we could construct the assignment matrix from `y`:
 ```
 A = np.zeros((N, M))
 for j in range(M):
     A[y[j], j] = 1
 ```
```

### Comparing `lapx-0.5.8/README.md` & `lapx-0.5.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,88 @@
 [![Test Simple](https://github.com/rathaROG/lapx/actions/workflows/test_simple.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/test_simple.yaml)
 [![Benchmark](https://github.com/rathaROG/lapx/actions/workflows/benchmark.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/benchmark.yaml)
 [![Test PyPI Build](https://github.com/rathaROG/lapx/actions/workflows/prepublish.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/prepublish.yaml)
 [![Publish to PyPI](https://github.com/rathaROG/lapx/actions/workflows/publish.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/publish.yaml)
 
 # Linear Assignment Problem Solver
 
-`lapx` basically is Tomas Kazmar's [`gatagat/lap`](https://github.com/gatagat/lap) with support for all Windows/Linux/macOS and Python 3.7/3.8/3.9/3.10/3.11/3.12.
+`lapx` basically is Tomas Kazmar's [`gatagat/lap`](https://github.com/gatagat/lap) with support for all Windows/Linux/macOS and Python 3.7-3.12. 
 
-* Based on: [[ed04ab7752]](https://github.com/gatagat/lap/tree/ed04ab7752c7c9688ddcbae534633f34ce04361f)
-* License: BSD-2-Clause, see [`LICENSE`](LICENSE) @[`gatagat`](https://github.com/gatagat)
+## 💽 Installation
 
-## 💽 Installation:
+### Install from [PyPI](https://pypi.org/project/lapx/):
 
-* Install from [PyPI](https://pypi.org/project/lapx/):
+[![PyPI version](https://badge.fury.io/py/lapx.svg)](https://badge.fury.io/py/lapx)
+[![Downloads](https://static.pepy.tech/badge/lapx)](https://pepy.tech/project/lapx)
+[![Downloads](https://static.pepy.tech/badge/lapx/month)](https://pepy.tech/project/lapx)
 
-  ```
-  pip install lapx
-  ```
-
-  | **Pre-built Wheels** 🛞 | **Windows** ✅ | **Linux** ✅ | **macOS** ✅ |
-  |:---:|:---:|:---:|:---:|
-  | Python v3.7 | AMD64 | x86_64/aarch64 ² | x86_64 |
-  | Python v3.8 | AMD64 | x86_64/aarch64 ² | x86_64/arm64 |
-  | Python v3.9 | AMD64/ARM64 ¹ | x86_64/aarch64 ² | x86_64/arm64 |
-  | Python v3.10 | AMD64/ARM64 ¹ | x86_64/aarch64 ² | x86_64/arm64 |
-  | Python v3.11 | AMD64/ARM64 ¹ | x86_64/aarch64 ² | x86_64/arm64 |
-  | Python v3.12 | AMD64/ARM64 ¹ | x86_64/aarch64 ² | x86_64/arm64 |
-
-  <sup>¹ Windows ARM64 is experimental.</sup><br>
-  <sup>² Linux now includes both `manylinux` and `musllinux`.</sup><br>
-
-* Or install from GitHub repo directly (Require C++ compiler):
-
-  ```
-  pip install git+https://github.com/rathaROG/lapx.git
-  ```
-
-* Or clone and build on your local machine (Require C++ compiler):
+```
+pip install lapx
+```
 
-  <details><summary><ins>Click here to expand!</ins></summary>
-  
-  ```
-  git clone https://github.com/rathaROG/lapx.git
-  cd lapx
-  python -m pip install --upgrade pip
-  pip install "setuptools>=67.2.0"
-  pip install wheel build
-  python -m build --wheel
-  cd dist
-  ```
-  
-  </details>
+| **Pre-built Wheels** 🛞 | **Windows** ✅ | **Linux** ✅ | **macOS** ✅ |
+|:---:|:---:|:---:|:---:|
+| Python 3.7 | AMD64 | x86_64/aarch64 | x86_64 |
+| Python 3.8 | AMD64 | x86_64/aarch64 | x86_64/arm64 |
+| Python 3.9-3.12 | AMD64/ARM64 ¹ | x86_64/aarch64 | x86_64/arm64 |
 
-## 🧪 Usage:
+<sup>¹ Windows ARM64 is experimental.</sup><br>
 
-* `lapx` is just the name for package distribution.
-* The same as `lap`, use `import lap` to import; for example:
+<details><summary>Click here to expand!</summary>
 
-  ```
-  import lap
-  import numpy as np
-  print(lap.lapjv(np.random.rand(4, 5), extend_cost=True))
-  ```
+### Install from GitHub repo (Require C++ compiler):
 
-<br />
+```
+pip install git+https://github.com/rathaROG/lapx.git
+```
 
-<details><summary>Click here to show more...</summary>
+### Build and install (Require C++ compiler):
 
-<br />
+```
+git clone https://github.com/rathaROG/lapx.git
+cd lapx
+pip install "setuptools>=67.8.0"
+pip install wheel build
+python -m build --wheel
+cd dist
+```
 
-lap: Linear Assignment Problem solver
-=====================================
+</details>
 
-**lap** is a [linear assignment
-problem](https://en.wikipedia.org/wiki/Assignment_problem) solver using
-Jonker-Volgenant algorithm for dense (LAPJV [1]) or sparse (LAPMOD [2])
-matrices.
+## 🧪 Usage
 
-Both algorithms are implemented from scratch based solely on the papers [1,2]
-and the public domain Pascal implementation provided by A. Volgenant [3].
+`lapx` is just the name for package distribution. The same as `lap`, use `import lap` to import; for example:
 
-In my tests the LAPMOD implementation seems to be faster than the LAPJV
-implementation for matrices with a side of more than ~5000 and with less than
-50% finite coefficients.
+```
+import lap
+import numpy as np
+print(lap.lapjv(np.random.rand(4, 5), extend_cost=True))
+```
 
-[1] R. Jonker and A. Volgenant, "A Shortest Augmenting Path Algorithm for Dense
-and Sparse Linear Assignment Problems", Computing 38, 325-340 (1987)<br>
-[2] A. Volgenant, "Linear and Semi-Assignment Problems: A Core Oriented
-Approach", Computer Ops Res. 23, 917-932 (1996)<br>
-[3] http://www.assignmentproblems.com/LAPJV.htm
+## 🔎 More about LAP
 
+<details><summary>Click here to expand!</summary><br>
 
-### Usage
+Tomas Kazmar's [`gatagat/lap`](https://github.com/gatagat/lap) is a [linear assignment problem](https://en.wikipedia.org/wiki/Assignment_problem) solver using Jonker-Volgenant algorithm for dense LAPJV ¹ or sparse LAPMOD ² matrices. Both algorithms are implemented from scratch based solely on the papers ¹˒² and the public domain Pascal implementation provided by A. Volgenant ³. The LAPMOD implementation seems to be faster than the LAPJV implementation for matrices with a side of more than ~5000 and with less than 50% finite coefficients.
 
-```
-cost, x, y = lap.lapjv(C)
-```
+<sup>¹ R. Jonker and A. Volgenant, "A Shortest Augmenting Path Algorithm for Dense and Sparse Linear Assignment Problems", Computing 38, 325-340 (1987) </sup><br>
+<sup>² A. Volgenant, "Linear and Semi-Assignment Problems: A Core Oriented Approach", Computer Ops Res. 23, 917-932 (1996) </sup><br>
+<sup>³ http://www.assignmentproblems.com/LAPJV.htm </sup><br>
+  
+### `cost, x, y = lap.lapjv(C)`
 
-The function `lapjv(C)` returns the assignment cost (`cost`) and two arrays, `x, y`. If cost matrix `C` has shape N x M, then `x` is a size-N array specifying to which column is row is assigned, and `y` is a size-M array specifying to which row each column is assigned. For example, an output of `x = [1, 0]` indicates that row 0 is assigned to column 1 and row 1 is assigned to column 0. Similarly, an output of `x = [2, 1, 0]` indicates that row 0 is assigned to column 2, row 1 is assigned to column 1, and row 2 is assigned to column 0.
+The function `lapjv(C)` returns the assignment cost `cost` and two arrays `x` and `y`. If cost matrix `C` has shape NxM, then `x` is a size-N array specifying to which column is row is assigned, and `y` is a size-M array specifying to which row each column is assigned. For example, an output of `x = [1, 0]` indicates that row 0 is assigned to column 1 and row 1 is assigned to column 0. Similarly, an output of `x = [2, 1, 0]` indicates that row 0 is assigned to column 2, row 1 is assigned to column 1, and row 2 is assigned to column 0.
 
 Note that this function *does not* return the assignment matrix (as done by scipy's [`linear_sum_assignment`](https://docs.scipy.org/doc/scipy-0.18.1/reference/generated/scipy.optimize.linear_sum_assignment.html) and lapsolver's [`solve dense`](https://github.com/cheind/py-lapsolver)). The assignment matrix can be constructed from `x` as follows:
 ```
 A = np.zeros((N, M))
 for i in range(N):
     A[i, x[i]] = 1
 ```
+
 Equivalently, we could construct the assignment matrix from `y`:
 ```
 A = np.zeros((N, M))
 for j in range(M):
     A[y[j], j] = 1
 ```
```

### Comparing `lapx-0.5.8/_lapjv_src/_lapjv.cpp` & `lapx-0.5.9/_lapjv_src/_lapjv.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1556,177 +1556,177 @@
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1755,42 +1755,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3288,261 +3288,261 @@
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
 #define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
 #define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
 #define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
 #define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
 /* #### Code section: module_code ### */
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3551,29 +3551,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3584,15 +3584,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3601,29 +3601,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3634,15 +3634,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3651,29 +3651,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3684,15 +3684,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3701,29 +3701,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3734,15 +3734,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3751,29 +3751,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3784,217 +3784,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4010,15 +4010,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4026,68 +4026,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4095,15 +4095,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4118,15 +4118,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4142,15 +4142,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4158,68 +4158,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4227,15 +4227,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4250,15 +4250,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4274,15 +4274,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4290,68 +4290,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4359,15 +4359,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4382,170 +4382,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -5600,15 +5600,15 @@
     }
 
     /* "_lapjv.pyx":119
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')
  *         raise RuntimeError('Unknown error (lapjv_internal returned %d).' % ret)             # <<<<<<<<<<<<<<
  * 
- * 
+ *     cdef double opt = np.nan
  */
     __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_ret); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = PyUnicode_Format(__pyx_kp_u_Unknown_error_lapjv_internal_ret, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 119, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
@@ -5623,103 +5623,103 @@
  *     free(cost_ptr)
  *     if ret != 0:             # <<<<<<<<<<<<<<
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')
  */
   }
 
-  /* "_lapjv.pyx":122
- * 
+  /* "_lapjv.pyx":121
+ *         raise RuntimeError('Unknown error (lapjv_internal returned %d).' % ret)
  * 
  *     cdef double opt = np.nan             # <<<<<<<<<<<<<<
  *     if cost_limit < np.inf or extend_cost:
  *         x_c[x_c >= n_cols] = -1
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_nan); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_nan); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_opt = __pyx_t_21;
 
-  /* "_lapjv.pyx":123
+  /* "_lapjv.pyx":122
  * 
  *     cdef double opt = np.nan
  *     if cost_limit < np.inf or extend_cost:             # <<<<<<<<<<<<<<
  *         x_c[x_c >= n_cols] = -1
  *         y_c[y_c >= n_rows] = -1
  */
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_cost_limit); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_cost_limit); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_inf); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_inf); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_5, __pyx_t_6, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_5, __pyx_t_6, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_22 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_22 < 0))) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_22 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_22 < 0))) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (!__pyx_t_22) {
   } else {
     __pyx_t_2 = __pyx_t_22;
     goto __pyx_L12_bool_binop_done;
   }
   __pyx_t_22 = (__pyx_v_extend_cost != 0);
   __pyx_t_2 = __pyx_t_22;
   __pyx_L12_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "_lapjv.pyx":124
+    /* "_lapjv.pyx":123
  *     cdef double opt = np.nan
  *     if cost_limit < np.inf or extend_cost:
  *         x_c[x_c >= n_cols] = -1             # <<<<<<<<<<<<<<
  *         y_c[y_c >= n_rows] = -1
  *         x_c = x_c[:n_rows]
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 124, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_t_4, Py_GE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 124, __pyx_L1_error)
+    __pyx_t_6 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_t_4, Py_GE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 123, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_x_c), __pyx_t_6, __pyx_int_neg_1) < 0))) __PYX_ERR(0, 124, __pyx_L1_error)
+    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_x_c), __pyx_t_6, __pyx_int_neg_1) < 0))) __PYX_ERR(0, 123, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "_lapjv.pyx":125
+    /* "_lapjv.pyx":124
  *     if cost_limit < np.inf or extend_cost:
  *         x_c[x_c >= n_cols] = -1
  *         y_c[y_c >= n_rows] = -1             # <<<<<<<<<<<<<<
  *         x_c = x_c[:n_rows]
  *         y_c = y_c[:n_cols]
  */
-    __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 124, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = PyObject_RichCompare(((PyObject *)__pyx_v_y_c), __pyx_t_6, Py_GE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(((PyObject *)__pyx_v_y_c), __pyx_t_6, Py_GE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 124, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_y_c), __pyx_t_4, __pyx_int_neg_1) < 0))) __PYX_ERR(0, 125, __pyx_L1_error)
+    if (unlikely((PyObject_SetItem(((PyObject *)__pyx_v_y_c), __pyx_t_4, __pyx_int_neg_1) < 0))) __PYX_ERR(0, 124, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "_lapjv.pyx":126
+    /* "_lapjv.pyx":125
  *         x_c[x_c >= n_cols] = -1
  *         y_c[y_c >= n_rows] = -1
  *         x_c = x_c[:n_rows]             # <<<<<<<<<<<<<<
  *         y_c = y_c[:n_cols]
  *         if return_cost:
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = PySlice_New(Py_None, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __pyx_t_6 = PySlice_New(Py_None, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_x_c), __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_x_c), __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 126, __pyx_L1_error)
+    if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 125, __pyx_L1_error)
     __pyx_t_19 = ((PyArrayObject *)__pyx_t_4);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_x_c.rcbuffer->pybuffer);
       __pyx_t_1 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_19, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_1 < 0)) {
         PyErr_Fetch(&__pyx_t_11, &__pyx_t_12, &__pyx_t_13);
@@ -5728,36 +5728,36 @@
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_11, __pyx_t_12, __pyx_t_13);
         }
         __pyx_t_11 = __pyx_t_12 = __pyx_t_13 = 0;
       }
       __pyx_pybuffernd_x_c.diminfo[0].strides = __pyx_pybuffernd_x_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_x_c.diminfo[0].shape = __pyx_pybuffernd_x_c.rcbuffer->pybuffer.shape[0];
-      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 126, __pyx_L1_error)
+      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 125, __pyx_L1_error)
     }
     __pyx_t_19 = 0;
     __Pyx_DECREF_SET(__pyx_v_x_c, ((PyArrayObject *)__pyx_t_4));
     __pyx_t_4 = 0;
 
-    /* "_lapjv.pyx":127
+    /* "_lapjv.pyx":126
  *         y_c[y_c >= n_rows] = -1
  *         x_c = x_c[:n_rows]
  *         y_c = y_c[:n_cols]             # <<<<<<<<<<<<<<
  *         if return_cost:
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 127, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint_t(__pyx_v_n_cols); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = PySlice_New(Py_None, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 127, __pyx_L1_error)
+    __pyx_t_6 = PySlice_New(Py_None, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_y_c), __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 127, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_y_c), __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 127, __pyx_L1_error)
+    if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 126, __pyx_L1_error)
     __pyx_t_20 = ((PyArrayObject *)__pyx_t_4);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_y_c.rcbuffer->pybuffer);
       __pyx_t_1 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_20, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_1 < 0)) {
         PyErr_Fetch(&__pyx_t_13, &__pyx_t_12, &__pyx_t_11);
@@ -5766,43 +5766,43 @@
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_13, __pyx_t_12, __pyx_t_11);
         }
         __pyx_t_13 = __pyx_t_12 = __pyx_t_11 = 0;
       }
       __pyx_pybuffernd_y_c.diminfo[0].strides = __pyx_pybuffernd_y_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_y_c.diminfo[0].shape = __pyx_pybuffernd_y_c.rcbuffer->pybuffer.shape[0];
-      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 127, __pyx_L1_error)
+      if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 126, __pyx_L1_error)
     }
     __pyx_t_20 = 0;
     __Pyx_DECREF_SET(__pyx_v_y_c, ((PyArrayObject *)__pyx_t_4));
     __pyx_t_4 = 0;
 
-    /* "_lapjv.pyx":128
+    /* "_lapjv.pyx":127
  *         x_c = x_c[:n_rows]
  *         y_c = y_c[:n_cols]
  *         if return_cost:             # <<<<<<<<<<<<<<
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  *     elif return_cost:
  */
     __pyx_t_2 = (__pyx_v_return_cost != 0);
     if (__pyx_t_2) {
 
-      /* "_lapjv.pyx":129
+      /* "_lapjv.pyx":128
  *         y_c = y_c[:n_cols]
  *         if return_cost:
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()             # <<<<<<<<<<<<<<
  *     elif return_cost:
  *         opt = cost_c[np.arange(n_rows), x_c].sum()
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_nonzero); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_nonzero); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_int_neg_1, Py_NE); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __pyx_t_5 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_int_neg_1, Py_NE); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
       __pyx_t_7 = NULL;
       __pyx_t_1 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -5814,37 +5814,37 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
         __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 129, __pyx_L1_error)
+        if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 128, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
-      __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_6, 0, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_6, 0, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_int_neg_1, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 129, __pyx_L1_error)
-      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_x_c), __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __pyx_t_6 = PyObject_RichCompare(((PyObject *)__pyx_v_x_c), __pyx_int_neg_1, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 128, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_x_c), __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_3);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error);
       __Pyx_GIVEREF(__pyx_t_5);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_5)) __PYX_ERR(0, 129, __pyx_L1_error);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error);
       __pyx_t_3 = 0;
       __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_cost_c), __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_cost_c), __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_sum); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_sum); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_5 = NULL;
       __pyx_t_1 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
@@ -5857,64 +5857,64 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_1, 0+__pyx_t_1);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 129, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       }
-      __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 129, __pyx_L1_error)
+      __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 128, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_v_opt = __pyx_t_21;
 
-      /* "_lapjv.pyx":128
+      /* "_lapjv.pyx":127
  *         x_c = x_c[:n_rows]
  *         y_c = y_c[:n_cols]
  *         if return_cost:             # <<<<<<<<<<<<<<
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  *     elif return_cost:
  */
     }
 
-    /* "_lapjv.pyx":123
+    /* "_lapjv.pyx":122
  * 
  *     cdef double opt = np.nan
  *     if cost_limit < np.inf or extend_cost:             # <<<<<<<<<<<<<<
  *         x_c[x_c >= n_cols] = -1
  *         y_c[y_c >= n_rows] = -1
  */
     goto __pyx_L11;
   }
 
-  /* "_lapjv.pyx":130
+  /* "_lapjv.pyx":129
  *         if return_cost:
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  *     elif return_cost:             # <<<<<<<<<<<<<<
  *         opt = cost_c[np.arange(n_rows), x_c].sum()
  * 
  */
   __pyx_t_2 = (__pyx_v_return_cost != 0);
   if (__pyx_t_2) {
 
-    /* "_lapjv.pyx":131
+    /* "_lapjv.pyx":130
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  *     elif return_cost:
  *         opt = cost_c[np.arange(n_rows), x_c].sum()             # <<<<<<<<<<<<<<
  * 
  *     if return_cost:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_arange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_arange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_uint_t(__pyx_v_n_rows); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_7 = NULL;
     __pyx_t_1 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_7)) {
@@ -5927,30 +5927,30 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
       __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 131, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 130, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_6);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6)) __PYX_ERR(0, 131, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6)) __PYX_ERR(0, 130, __pyx_L1_error);
     __Pyx_INCREF((PyObject *)__pyx_v_x_c);
     __Pyx_GIVEREF((PyObject *)__pyx_v_x_c);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, ((PyObject *)__pyx_v_x_c))) __PYX_ERR(0, 131, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, ((PyObject *)__pyx_v_x_c))) __PYX_ERR(0, 130, __pyx_L1_error);
     __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_cost_c), __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_cost_c), __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_sum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_sum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     __pyx_t_1 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
@@ -5963,93 +5963,93 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, NULL};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_1, 0+__pyx_t_1);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_21 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_21 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_opt = __pyx_t_21;
 
-    /* "_lapjv.pyx":130
+    /* "_lapjv.pyx":129
  *         if return_cost:
  *             opt = cost_c[np.nonzero(x_c != -1)[0], x_c[x_c != -1]].sum()
  *     elif return_cost:             # <<<<<<<<<<<<<<
  *         opt = cost_c[np.arange(n_rows), x_c].sum()
  * 
  */
   }
   __pyx_L11:;
 
-  /* "_lapjv.pyx":133
+  /* "_lapjv.pyx":132
  *         opt = cost_c[np.arange(n_rows), x_c].sum()
  * 
  *     if return_cost:             # <<<<<<<<<<<<<<
  *         return opt, x_c, y_c
  *     else:
  */
   __pyx_t_2 = (__pyx_v_return_cost != 0);
   if (__pyx_t_2) {
 
-    /* "_lapjv.pyx":134
+    /* "_lapjv.pyx":133
  * 
  *     if return_cost:
  *         return opt, x_c, y_c             # <<<<<<<<<<<<<<
  *     else:
  *         return x_c, y_c
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = PyFloat_FromDouble(__pyx_v_opt); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 134, __pyx_L1_error)
+    __pyx_t_4 = PyFloat_FromDouble(__pyx_v_opt); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 134, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 134, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error);
     __Pyx_INCREF((PyObject *)__pyx_v_x_c);
     __Pyx_GIVEREF((PyObject *)__pyx_v_x_c);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, ((PyObject *)__pyx_v_x_c))) __PYX_ERR(0, 134, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, ((PyObject *)__pyx_v_x_c))) __PYX_ERR(0, 133, __pyx_L1_error);
     __Pyx_INCREF((PyObject *)__pyx_v_y_c);
     __Pyx_GIVEREF((PyObject *)__pyx_v_y_c);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 2, ((PyObject *)__pyx_v_y_c))) __PYX_ERR(0, 134, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 2, ((PyObject *)__pyx_v_y_c))) __PYX_ERR(0, 133, __pyx_L1_error);
     __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "_lapjv.pyx":133
+    /* "_lapjv.pyx":132
  *         opt = cost_c[np.arange(n_rows), x_c].sum()
  * 
  *     if return_cost:             # <<<<<<<<<<<<<<
  *         return opt, x_c, y_c
  *     else:
  */
   }
 
-  /* "_lapjv.pyx":136
+  /* "_lapjv.pyx":135
  *         return opt, x_c, y_c
  *     else:
  *         return x_c, y_c             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF((PyObject *)__pyx_v_x_c);
     __Pyx_GIVEREF((PyObject *)__pyx_v_x_c);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_x_c))) __PYX_ERR(0, 136, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_x_c))) __PYX_ERR(0, 135, __pyx_L1_error);
     __Pyx_INCREF((PyObject *)__pyx_v_y_c);
     __Pyx_GIVEREF((PyObject *)__pyx_v_y_c);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, ((PyObject *)__pyx_v_y_c))) __PYX_ERR(0, 136, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, ((PyObject *)__pyx_v_y_c))) __PYX_ERR(0, 135, __pyx_L1_error);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
   /* "_lapjv.pyx":42
  * # https://github.com/rathaROG/lapx/pull/7
@@ -6089,15 +6089,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_x_c);
   __Pyx_XDECREF((PyObject *)__pyx_v_y_c);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_lapjv.pyx":139
+/* "_lapjv.pyx":138
  * 
  * 
  * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
  * def _lapmod(const uint_t n,
  */
 
@@ -6107,28 +6107,28 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum__fp_t(__Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_fp_version); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__fp_t(__Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_fp_version); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error);
   __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, Py_None)) __PYX_ERR(0, 139, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, Py_None)) __PYX_ERR(0, 138, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6205,99 +6205,99 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 138, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cc)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 138, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 1); __PYX_ERR(0, 139, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 1); __PYX_ERR(0, 138, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ii)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 138, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 2); __PYX_ERR(0, 139, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 2); __PYX_ERR(0, 138, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kk)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 138, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 3); __PYX_ERR(0, 139, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, 3); __PYX_ERR(0, 138, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fp_version);
           if (value) { values[4] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 138, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_lapmod") < 0)) __PYX_ERR(0, 139, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_lapmod") < 0)) __PYX_ERR(0, 138, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_n = __Pyx_PyInt_As_uint_t(values[0]); if (unlikely((__pyx_v_n == ((uint_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 141, __pyx_L3_error)
+    __pyx_v_n = __Pyx_PyInt_As_uint_t(values[0]); if (unlikely((__pyx_v_n == ((uint_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 140, __pyx_L3_error)
     __pyx_v_cc = ((PyArrayObject *)values[1]);
     __pyx_v_ii = ((PyArrayObject *)values[2]);
     __pyx_v_kk = ((PyArrayObject *)values[3]);
     if (values[4]) {
-      __pyx_v_fp_version = ((enum fp_t)__Pyx_PyInt_As_enum__fp_t(values[4])); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 145, __pyx_L3_error)
+      __pyx_v_fp_version = ((enum fp_t)__Pyx_PyInt_As_enum__fp_t(values[4])); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 144, __pyx_L3_error)
     } else {
       __pyx_v_fp_version = __pyx_dynamic_args->__pyx_arg_fp_version;
     }
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, __pyx_nargs); __PYX_ERR(0, 139, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_lapmod", 0, 4, 5, __pyx_nargs); __PYX_ERR(0, 138, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("_lapjv._lapmod", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cc), __pyx_ptype_5numpy_ndarray, 0, "cc", 0))) __PYX_ERR(0, 142, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ii), __pyx_ptype_5numpy_ndarray, 0, "ii", 0))) __PYX_ERR(0, 143, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_kk), __pyx_ptype_5numpy_ndarray, 0, "kk", 0))) __PYX_ERR(0, 144, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cc), __pyx_ptype_5numpy_ndarray, 0, "cc", 0))) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ii), __pyx_ptype_5numpy_ndarray, 0, "ii", 0))) __PYX_ERR(0, 142, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_kk), __pyx_ptype_5numpy_ndarray, 0, "kk", 0))) __PYX_ERR(0, 143, __pyx_L1_error)
   __pyx_r = __pyx_pf_6_lapjv_2_lapmod(__pyx_self, __pyx_v_n, __pyx_v_cc, __pyx_v_ii, __pyx_v_kk, __pyx_v_fp_version);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -6367,372 +6367,372 @@
   __pyx_pybuffernd_x_c.data = NULL;
   __pyx_pybuffernd_x_c.rcbuffer = &__pyx_pybuffer_x_c;
   __pyx_pybuffer_y_c.pybuffer.buf = NULL;
   __pyx_pybuffer_y_c.refcount = 0;
   __pyx_pybuffernd_y_c.data = NULL;
   __pyx_pybuffernd_y_c.rcbuffer = &__pyx_pybuffer_y_c;
 
-  /* "_lapjv.pyx":148
+  /* "_lapjv.pyx":147
  *     """Internal function called from lapmod(..., fast=True)."""
  *     cdef cnp.ndarray[cnp.double_t, ndim=1, mode='c'] cc_c = \
  *         np.ascontiguousarray(cc, dtype=np.double)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[uint_t, ndim=1, mode='c'] ii_c = \
  *         np.ascontiguousarray(ii, dtype=np.uint32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF((PyObject *)__pyx_v_cc);
   __Pyx_GIVEREF((PyObject *)__pyx_v_cc);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_cc))) __PYX_ERR(0, 148, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_cc))) __PYX_ERR(0, 147, __pyx_L1_error);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 148, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 147, __pyx_L1_error)
   __pyx_t_6 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cc_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_5numpy_double_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_cc_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_cc_c.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 147, __pyx_L1_error)
+      __PYX_ERR(0, 146, __pyx_L1_error)
     } else {__pyx_pybuffernd_cc_c.diminfo[0].strides = __pyx_pybuffernd_cc_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_cc_c.diminfo[0].shape = __pyx_pybuffernd_cc_c.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_6 = 0;
   __pyx_v_cc_c = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "_lapjv.pyx":150
+  /* "_lapjv.pyx":149
  *         np.ascontiguousarray(cc, dtype=np.double)
  *     cdef cnp.ndarray[uint_t, ndim=1, mode='c'] ii_c = \
  *         np.ascontiguousarray(ii, dtype=np.uint32)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[uint_t, ndim=1, mode='c'] kk_c = \
  *         np.ascontiguousarray(kk, dtype=np.uint32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF((PyObject *)__pyx_v_ii);
   __Pyx_GIVEREF((PyObject *)__pyx_v_ii);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject *)__pyx_v_ii))) __PYX_ERR(0, 150, __pyx_L1_error);
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject *)__pyx_v_ii))) __PYX_ERR(0, 149, __pyx_L1_error);
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 150, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 149, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ii_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn_uint_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_ii_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_ii_c.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 149, __pyx_L1_error)
+      __PYX_ERR(0, 148, __pyx_L1_error)
     } else {__pyx_pybuffernd_ii_c.diminfo[0].strides = __pyx_pybuffernd_ii_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_ii_c.diminfo[0].shape = __pyx_pybuffernd_ii_c.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_ii_c = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "_lapjv.pyx":152
+  /* "_lapjv.pyx":151
  *         np.ascontiguousarray(ii, dtype=np.uint32)
  *     cdef cnp.ndarray[uint_t, ndim=1, mode='c'] kk_c = \
  *         np.ascontiguousarray(kk, dtype=np.uint32)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[int_t, ndim=1, mode='c'] x_c = \
  *         np.empty((n,), dtype=np.int32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF((PyObject *)__pyx_v_kk);
   __Pyx_GIVEREF((PyObject *)__pyx_v_kk);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)__pyx_v_kk))) __PYX_ERR(0, 152, __pyx_L1_error);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 152, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)__pyx_v_kk))) __PYX_ERR(0, 151, __pyx_L1_error);
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 152, __pyx_L1_error)
+  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 151, __pyx_L1_error)
   __pyx_t_8 = ((PyArrayObject *)__pyx_t_2);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_kk_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn_uint_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_kk_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_kk_c.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 151, __pyx_L1_error)
+      __PYX_ERR(0, 150, __pyx_L1_error)
     } else {__pyx_pybuffernd_kk_c.diminfo[0].strides = __pyx_pybuffernd_kk_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_kk_c.diminfo[0].shape = __pyx_pybuffernd_kk_c.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_8 = 0;
   __pyx_v_kk_c = ((PyArrayObject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "_lapjv.pyx":154
+  /* "_lapjv.pyx":153
  *         np.ascontiguousarray(kk, dtype=np.uint32)
  *     cdef cnp.ndarray[int_t, ndim=1, mode='c'] x_c = \
  *         np.empty((n,), dtype=np.int32)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[int_t, ndim=1, mode='c'] y_c = \
  *         np.empty((n,), dtype=np.int32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error);
   __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4)) __PYX_ERR(0, 154, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4)) __PYX_ERR(0, 153, __pyx_L1_error);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 154, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 153, __pyx_L1_error)
   __pyx_t_9 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_x_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_x_c.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 153, __pyx_L1_error)
+      __PYX_ERR(0, 152, __pyx_L1_error)
     } else {__pyx_pybuffernd_x_c.diminfo[0].strides = __pyx_pybuffernd_x_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_x_c.diminfo[0].shape = __pyx_pybuffernd_x_c.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_9 = 0;
   __pyx_v_x_c = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "_lapjv.pyx":156
+  /* "_lapjv.pyx":155
  *         np.empty((n,), dtype=np.int32)
  *     cdef cnp.ndarray[int_t, ndim=1, mode='c'] y_c = \
  *         np.empty((n,), dtype=np.int32)             # <<<<<<<<<<<<<<
  * 
  *     cdef int_t ret = lapmod_internal(n, &cc_c[0], &ii_c[0], &kk_c[0],
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_uint_t(__pyx_v_n); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error);
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 156, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 156, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 155, __pyx_L1_error)
   __pyx_t_10 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_10, &__Pyx_TypeInfo_nn_int_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_y_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_y_c.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 155, __pyx_L1_error)
+      __PYX_ERR(0, 154, __pyx_L1_error)
     } else {__pyx_pybuffernd_y_c.diminfo[0].strides = __pyx_pybuffernd_y_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_y_c.diminfo[0].shape = __pyx_pybuffernd_y_c.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_10 = 0;
   __pyx_v_y_c = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "_lapjv.pyx":158
+  /* "_lapjv.pyx":157
  *         np.empty((n,), dtype=np.int32)
  * 
  *     cdef int_t ret = lapmod_internal(n, &cc_c[0], &ii_c[0], &kk_c[0],             # <<<<<<<<<<<<<<
  *                                      &x_c[0], &y_c[0], fp_version)
  *     if ret != 0:
  */
   __pyx_t_11 = 0;
   __pyx_t_12 = 0;
   __pyx_t_13 = 0;
 
-  /* "_lapjv.pyx":159
+  /* "_lapjv.pyx":158
  * 
  *     cdef int_t ret = lapmod_internal(n, &cc_c[0], &ii_c[0], &kk_c[0],
  *                                      &x_c[0], &y_c[0], fp_version)             # <<<<<<<<<<<<<<
  *     if ret != 0:
  *         if ret == -1:
  */
   __pyx_t_14 = 0;
   __pyx_t_15 = 0;
 
-  /* "_lapjv.pyx":158
+  /* "_lapjv.pyx":157
  *         np.empty((n,), dtype=np.int32)
  * 
  *     cdef int_t ret = lapmod_internal(n, &cc_c[0], &ii_c[0], &kk_c[0],             # <<<<<<<<<<<<<<
  *                                      &x_c[0], &y_c[0], fp_version)
  *     if ret != 0:
  */
   __pyx_v_ret = lapmod_internal(__pyx_v_n, (&(*__Pyx_BufPtrCContig1d(__pyx_t_5numpy_double_t *, __pyx_pybuffernd_cc_c.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_cc_c.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(uint_t *, __pyx_pybuffernd_ii_c.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_ii_c.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(uint_t *, __pyx_pybuffernd_kk_c.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_kk_c.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(int_t *, __pyx_pybuffernd_x_c.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_x_c.diminfo[0].strides))), (&(*__Pyx_BufPtrCContig1d(int_t *, __pyx_pybuffernd_y_c.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_y_c.diminfo[0].strides))), __pyx_v_fp_version);
 
-  /* "_lapjv.pyx":160
+  /* "_lapjv.pyx":159
  *     cdef int_t ret = lapmod_internal(n, &cc_c[0], &ii_c[0], &kk_c[0],
  *                                      &x_c[0], &y_c[0], fp_version)
  *     if ret != 0:             # <<<<<<<<<<<<<<
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')
  */
   __pyx_t_16 = (__pyx_v_ret != 0);
   if (__pyx_t_16) {
 
-    /* "_lapjv.pyx":161
+    /* "_lapjv.pyx":160
  *                                      &x_c[0], &y_c[0], fp_version)
  *     if ret != 0:
  *         if ret == -1:             # <<<<<<<<<<<<<<
  *             raise MemoryError('Out of memory.')
  *         raise RuntimeError('Unknown error (lapmod_internal returned %d).' % ret)
  */
     __pyx_t_16 = (__pyx_v_ret == -1L);
     if (unlikely(__pyx_t_16)) {
 
-      /* "_lapjv.pyx":162
+      /* "_lapjv.pyx":161
  *     if ret != 0:
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')             # <<<<<<<<<<<<<<
  *         raise RuntimeError('Unknown error (lapmod_internal returned %d).' % ret)
  * 
  */
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(0, 162, __pyx_L1_error)
+      __PYX_ERR(0, 161, __pyx_L1_error)
 
-      /* "_lapjv.pyx":161
+      /* "_lapjv.pyx":160
  *                                      &x_c[0], &y_c[0], fp_version)
  *     if ret != 0:
  *         if ret == -1:             # <<<<<<<<<<<<<<
  *             raise MemoryError('Out of memory.')
  *         raise RuntimeError('Unknown error (lapmod_internal returned %d).' % ret)
  */
     }
 
-    /* "_lapjv.pyx":163
+    /* "_lapjv.pyx":162
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')
  *         raise RuntimeError('Unknown error (lapmod_internal returned %d).' % ret)             # <<<<<<<<<<<<<<
  * 
  *     return x_c, y_c
  */
-    __pyx_t_1 = __Pyx_PyInt_From_int_t(__pyx_v_ret); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int_t(__pyx_v_ret); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyUnicode_Format(__pyx_kp_u_Unknown_error_lapmod_internal_re, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_2 = PyUnicode_Format(__pyx_kp_u_Unknown_error_lapmod_internal_re, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 163, __pyx_L1_error)
+    __PYX_ERR(0, 162, __pyx_L1_error)
 
-    /* "_lapjv.pyx":160
+    /* "_lapjv.pyx":159
  *     cdef int_t ret = lapmod_internal(n, &cc_c[0], &ii_c[0], &kk_c[0],
  *                                      &x_c[0], &y_c[0], fp_version)
  *     if ret != 0:             # <<<<<<<<<<<<<<
  *         if ret == -1:
  *             raise MemoryError('Out of memory.')
  */
   }
 
-  /* "_lapjv.pyx":165
+  /* "_lapjv.pyx":164
  *         raise RuntimeError('Unknown error (lapmod_internal returned %d).' % ret)
  * 
  *     return x_c, y_c             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF((PyObject *)__pyx_v_x_c);
   __Pyx_GIVEREF((PyObject *)__pyx_v_x_c);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_x_c))) __PYX_ERR(0, 165, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_x_c))) __PYX_ERR(0, 164, __pyx_L1_error);
   __Pyx_INCREF((PyObject *)__pyx_v_y_c);
   __Pyx_GIVEREF((PyObject *)__pyx_v_y_c);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)__pyx_v_y_c))) __PYX_ERR(0, 165, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)__pyx_v_y_c))) __PYX_ERR(0, 164, __pyx_L1_error);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_lapjv.pyx":139
+  /* "_lapjv.pyx":138
  * 
  * 
  * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
  * def _lapmod(const uint_t n,
  */
 
@@ -6874,26 +6874,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-gu45fola/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-5d50agxh/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 990, __pyx_L1_error)
@@ -6952,25 +6952,25 @@
  * def lapjv(cnp.ndarray cost not None, char extend_cost=False,
  */
   __pyx_tuple__8 = PyTuple_Pack(15, __pyx_n_s_cost, __pyx_n_s_extend_cost, __pyx_n_s_cost_limit, __pyx_n_s_return_cost, __pyx_n_s_cost_c, __pyx_n_s_cost_c_extended, __pyx_n_s_n_rows, __pyx_n_s_n_cols, __pyx_n_s_n, __pyx_n_s_cost_ptr, __pyx_n_s_i, __pyx_n_s_x_c, __pyx_n_s_y_c, __pyx_n_s_ret, __pyx_n_s_opt); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
   __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lapjv_src__lapjv_pyx, __pyx_n_s_lapjv, 42, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 42, __pyx_L1_error)
 
-  /* "_lapjv.pyx":139
+  /* "_lapjv.pyx":138
  * 
  * 
  * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
  * def _lapmod(const uint_t n,
  */
-  __pyx_tuple__10 = PyTuple_Pack(11, __pyx_n_s_n, __pyx_n_s_cc, __pyx_n_s_ii, __pyx_n_s_kk, __pyx_n_s_fp_version, __pyx_n_s_cc_c, __pyx_n_s_ii_c, __pyx_n_s_kk_c, __pyx_n_s_x_c, __pyx_n_s_y_c, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(11, __pyx_n_s_n, __pyx_n_s_cc, __pyx_n_s_ii, __pyx_n_s_kk, __pyx_n_s_fp_version, __pyx_n_s_cc_c, __pyx_n_s_ii_c, __pyx_n_s_kk_c, __pyx_n_s_x_c, __pyx_n_s_y_c, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lapjv_src__lapjv_pyx, __pyx_n_s_lapmod, 139, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lapjv_src__lapjv_pyx, __pyx_n_s_lapmod, 138, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -7480,41 +7480,41 @@
   __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_2)->__pyx_arg_cost_limit = __pyx_t_5;
   __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_6_lapjv_4__defaults__);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_lapjv, __pyx_t_2) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_lapjv.pyx":139
+  /* "_lapjv.pyx":138
  * 
  * 
  * @cython.boundscheck(False)             # <<<<<<<<<<<<<<
  * @cython.wraparound(False)
  * def _lapmod(const uint_t n,
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_lapjv_3_lapmod, 0, __pyx_n_s_lapmod, NULL, __pyx_n_s_lapjv_2, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_lapjv_3_lapmod, 0, __pyx_n_s_lapmod, NULL, __pyx_n_s_lapjv_2, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults1), 0)) __PYX_ERR(0, 139, __pyx_L1_error)
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults1), 0)) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "_lapjv.pyx":145
+  /* "_lapjv.pyx":144
  *             cnp.ndarray ii not None,
  *             cnp.ndarray kk not None,
  *             fp_t fp_version=FP_DYNAMIC):             # <<<<<<<<<<<<<<
  *     """Internal function called from lapmod(..., fast=True)."""
  *     cdef cnp.ndarray[cnp.double_t, ndim=1, mode='c'] cc_c = \
  */
   __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_t_2)->__pyx_arg_fp_version = FP_DYNAMIC;
   __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_6_lapjv_6__defaults__);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lapmod, __pyx_t_2) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lapmod, __pyx_t_2) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_lapjv.pyx":1
  * # Tomas Kazmar, 2012-2017, BSD 2-clause license, see LICENSE.             # <<<<<<<<<<<<<<
  * 
- * # Updated 2023/06/22 by rathaROG
+ * # Updated by rathaROG
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
```

### Comparing `lapx-0.5.8/_lapjv_src/_lapjv.pyx` & `lapx-0.5.9/_lapjv_src/_lapjv.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Tomas Kazmar, 2012-2017, BSD 2-clause license, see LICENSE.
 
-# Updated 2023/06/22 by rathaROG
+# Updated by rathaROG
 # Force compiling with Python 3 
 # cython: language_level=3
 
 import numpy as np
 cimport numpy as cnp
 cimport cython
 from libc.stdlib cimport malloc, free
@@ -114,15 +114,14 @@
     cdef int ret = lapjv_internal(n, cost_ptr, &x_c[0], &y_c[0])
     free(cost_ptr)
     if ret != 0:
         if ret == -1:
             raise MemoryError('Out of memory.')
         raise RuntimeError('Unknown error (lapjv_internal returned %d).' % ret)
 
-
     cdef double opt = np.nan
     if cost_limit < np.inf or extend_cost:
         x_c[x_c >= n_cols] = -1
         y_c[y_c >= n_rows] = -1
         x_c = x_c[:n_rows]
         y_c = y_c[:n_cols]
         if return_cost:
```

### Comparing `lapx-0.5.8/_lapjv_src/lapjv.cpp` & `lapx-0.5.9/_lapjv_src/lapjv.cpp`

 * *Files identical despite different names*

### Comparing `lapx-0.5.8/_lapjv_src/lapjv.h` & `lapx-0.5.9/_lapjv_src/lapjv.h`

 * *Files identical despite different names*

### Comparing `lapx-0.5.8/_lapjv_src/lapmod.cpp` & `lapx-0.5.9/_lapjv_src/lapmod.cpp`

 * *Files identical despite different names*

### Comparing `lapx-0.5.8/lap/__init__.py` & `lapx-0.5.9/lap/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 lapjv
     Find optimal (minimum-cost) assignment for a dense cost matrix.
 lapmod
     Find optimal (minimum-cost) assignment for a sparse cost matrix.
 """
 
-__version__ = '0.5.8'
+__version__ = '0.5.9'
 
 from ._lapjv import (
     lapjv,
     LARGE_ as LARGE,
     FP_1_ as FP_1,
     FP_2_ as FP_2,
     FP_DYNAMIC_ as FP_DYNAMIC
```

### Comparing `lapx-0.5.8/lap/lapmod.py` & `lapx-0.5.9/lap/lapmod.py`

 * *Files identical despite different names*

### Comparing `lapx-0.5.8/lap/tests/cost_eps.csv.gz` & `lapx-0.5.9/lap/tests/cost_eps.csv.gz`

 * *Files identical despite different names*

### Comparing `lapx-0.5.8/lap/tests/test_arr_loop.py` & `lapx-0.5.9/lap/tests/test_arr_loop.py`

 * *Files identical despite different names*

### Comparing `lapx-0.5.8/lap/tests/test_lapjv.py` & `lapx-0.5.9/lap/tests/test_lapjv.py`

 * *Files identical despite different names*

### Comparing `lapx-0.5.8/lap/tests/test_lapmod.py` & `lapx-0.5.9/lap/tests/test_lapmod.py`

 * *Files identical despite different names*

### Comparing `lapx-0.5.8/lap/tests/test_utils.py` & `lapx-0.5.9/lap/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lapx-0.5.8/lapx.egg-info/PKG-INFO` & `lapx-0.5.9/lapx.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lapx
-Version: 0.5.8
+Version: 0.5.9
 Summary: Linear Assignment Problem solver (LAPJV/LAPMOD).
 Home-page: https://github.com/rathaROG/lapx
 Author: rathaROG
 License: BSD-2-Clause
 Keywords: Linear Assignment,LAPJV,LAPMOD,lap
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -28,124 +28,97 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Cython>=0.29.32
 Requires-Dist: numpy>=1.21.6
 
 [![Test Simple](https://github.com/rathaROG/lapx/actions/workflows/test_simple.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/test_simple.yaml)
 [![Benchmark](https://github.com/rathaROG/lapx/actions/workflows/benchmark.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/benchmark.yaml)
 [![Test PyPI Build](https://github.com/rathaROG/lapx/actions/workflows/prepublish.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/prepublish.yaml)
 [![Publish to PyPI](https://github.com/rathaROG/lapx/actions/workflows/publish.yaml/badge.svg)](https://github.com/rathaROG/lapx/actions/workflows/publish.yaml)
 
 # Linear Assignment Problem Solver
 
-`lapx` basically is Tomas Kazmar's [`gatagat/lap`](https://github.com/gatagat/lap) with support for all Windows/Linux/macOS and Python 3.7/3.8/3.9/3.10/3.11/3.12.
+`lapx` basically is Tomas Kazmar's [`gatagat/lap`](https://github.com/gatagat/lap) with support for all Windows/Linux/macOS and Python 3.7-3.12. 
 
-* Based on: [[ed04ab7752]](https://github.com/gatagat/lap/tree/ed04ab7752c7c9688ddcbae534633f34ce04361f)
-* License: BSD-2-Clause, see [`LICENSE`](LICENSE) @[`gatagat`](https://github.com/gatagat)
+## 💽 Installation
 
-## 💽 Installation:
+### Install from [PyPI](https://pypi.org/project/lapx/):
 
-* Install from [PyPI](https://pypi.org/project/lapx/):
+[![PyPI version](https://badge.fury.io/py/lapx.svg)](https://badge.fury.io/py/lapx)
+[![Downloads](https://static.pepy.tech/badge/lapx)](https://pepy.tech/project/lapx)
+[![Downloads](https://static.pepy.tech/badge/lapx/month)](https://pepy.tech/project/lapx)
 
-  ```
-  pip install lapx
-  ```
-
-  | **Pre-built Wheels** 🛞 | **Windows** ✅ | **Linux** ✅ | **macOS** ✅ |
-  |:---:|:---:|:---:|:---:|
-  | Python v3.7 | AMD64 | x86_64/aarch64 ² | x86_64 |
-  | Python v3.8 | AMD64 | x86_64/aarch64 ² | x86_64/arm64 |
-  | Python v3.9 | AMD64/ARM64 ¹ | x86_64/aarch64 ² | x86_64/arm64 |
-  | Python v3.10 | AMD64/ARM64 ¹ | x86_64/aarch64 ² | x86_64/arm64 |
-  | Python v3.11 | AMD64/ARM64 ¹ | x86_64/aarch64 ² | x86_64/arm64 |
-  | Python v3.12 | AMD64/ARM64 ¹ | x86_64/aarch64 ² | x86_64/arm64 |
-
-  <sup>¹ Windows ARM64 is experimental.</sup><br>
-  <sup>² Linux now includes both `manylinux` and `musllinux`.</sup><br>
-
-* Or install from GitHub repo directly (Require C++ compiler):
-
-  ```
-  pip install git+https://github.com/rathaROG/lapx.git
-  ```
-
-* Or clone and build on your local machine (Require C++ compiler):
+```
+pip install lapx
+```
 
-  <details><summary><ins>Click here to expand!</ins></summary>
-  
-  ```
-  git clone https://github.com/rathaROG/lapx.git
-  cd lapx
-  python -m pip install --upgrade pip
-  pip install "setuptools>=67.2.0"
-  pip install wheel build
-  python -m build --wheel
-  cd dist
-  ```
-  
-  </details>
+| **Pre-built Wheels** 🛞 | **Windows** ✅ | **Linux** ✅ | **macOS** ✅ |
+|:---:|:---:|:---:|:---:|
+| Python 3.7 | AMD64 | x86_64/aarch64 | x86_64 |
+| Python 3.8 | AMD64 | x86_64/aarch64 | x86_64/arm64 |
+| Python 3.9-3.12 | AMD64/ARM64 ¹ | x86_64/aarch64 | x86_64/arm64 |
 
-## 🧪 Usage:
+<sup>¹ Windows ARM64 is experimental.</sup><br>
 
-* `lapx` is just the name for package distribution.
-* The same as `lap`, use `import lap` to import; for example:
+<details><summary>Click here to expand!</summary>
 
-  ```
-  import lap
-  import numpy as np
-  print(lap.lapjv(np.random.rand(4, 5), extend_cost=True))
-  ```
+### Install from GitHub repo (Require C++ compiler):
 
-<br />
+```
+pip install git+https://github.com/rathaROG/lapx.git
+```
 
-<details><summary>Click here to show more...</summary>
+### Build and install (Require C++ compiler):
 
-<br />
+```
+git clone https://github.com/rathaROG/lapx.git
+cd lapx
+pip install "setuptools>=67.8.0"
+pip install wheel build
+python -m build --wheel
+cd dist
+```
 
-lap: Linear Assignment Problem solver
-=====================================
+</details>
 
-**lap** is a [linear assignment
-problem](https://en.wikipedia.org/wiki/Assignment_problem) solver using
-Jonker-Volgenant algorithm for dense (LAPJV [1]) or sparse (LAPMOD [2])
-matrices.
+## 🧪 Usage
 
-Both algorithms are implemented from scratch based solely on the papers [1,2]
-and the public domain Pascal implementation provided by A. Volgenant [3].
+`lapx` is just the name for package distribution. The same as `lap`, use `import lap` to import; for example:
 
-In my tests the LAPMOD implementation seems to be faster than the LAPJV
-implementation for matrices with a side of more than ~5000 and with less than
-50% finite coefficients.
+```
+import lap
+import numpy as np
+print(lap.lapjv(np.random.rand(4, 5), extend_cost=True))
+```
 
-[1] R. Jonker and A. Volgenant, "A Shortest Augmenting Path Algorithm for Dense
-and Sparse Linear Assignment Problems", Computing 38, 325-340 (1987)<br>
-[2] A. Volgenant, "Linear and Semi-Assignment Problems: A Core Oriented
-Approach", Computer Ops Res. 23, 917-932 (1996)<br>
-[3] http://www.assignmentproblems.com/LAPJV.htm
+## 🔎 More about LAP
 
+<details><summary>Click here to expand!</summary><br>
 
-### Usage
+Tomas Kazmar's [`gatagat/lap`](https://github.com/gatagat/lap) is a [linear assignment problem](https://en.wikipedia.org/wiki/Assignment_problem) solver using Jonker-Volgenant algorithm for dense LAPJV ¹ or sparse LAPMOD ² matrices. Both algorithms are implemented from scratch based solely on the papers ¹˒² and the public domain Pascal implementation provided by A. Volgenant ³. The LAPMOD implementation seems to be faster than the LAPJV implementation for matrices with a side of more than ~5000 and with less than 50% finite coefficients.
 
-```
-cost, x, y = lap.lapjv(C)
-```
+<sup>¹ R. Jonker and A. Volgenant, "A Shortest Augmenting Path Algorithm for Dense and Sparse Linear Assignment Problems", Computing 38, 325-340 (1987) </sup><br>
+<sup>² A. Volgenant, "Linear and Semi-Assignment Problems: A Core Oriented Approach", Computer Ops Res. 23, 917-932 (1996) </sup><br>
+<sup>³ http://www.assignmentproblems.com/LAPJV.htm </sup><br>
+  
+### `cost, x, y = lap.lapjv(C)`
 
-The function `lapjv(C)` returns the assignment cost (`cost`) and two arrays, `x, y`. If cost matrix `C` has shape N x M, then `x` is a size-N array specifying to which column is row is assigned, and `y` is a size-M array specifying to which row each column is assigned. For example, an output of `x = [1, 0]` indicates that row 0 is assigned to column 1 and row 1 is assigned to column 0. Similarly, an output of `x = [2, 1, 0]` indicates that row 0 is assigned to column 2, row 1 is assigned to column 1, and row 2 is assigned to column 0.
+The function `lapjv(C)` returns the assignment cost `cost` and two arrays `x` and `y`. If cost matrix `C` has shape NxM, then `x` is a size-N array specifying to which column is row is assigned, and `y` is a size-M array specifying to which row each column is assigned. For example, an output of `x = [1, 0]` indicates that row 0 is assigned to column 1 and row 1 is assigned to column 0. Similarly, an output of `x = [2, 1, 0]` indicates that row 0 is assigned to column 2, row 1 is assigned to column 1, and row 2 is assigned to column 0.
 
 Note that this function *does not* return the assignment matrix (as done by scipy's [`linear_sum_assignment`](https://docs.scipy.org/doc/scipy-0.18.1/reference/generated/scipy.optimize.linear_sum_assignment.html) and lapsolver's [`solve dense`](https://github.com/cheind/py-lapsolver)). The assignment matrix can be constructed from `x` as follows:
 ```
 A = np.zeros((N, M))
 for i in range(N):
     A[i, x[i]] = 1
 ```
+
 Equivalently, we could construct the assignment matrix from `y`:
 ```
 A = np.zeros((N, M))
 for j in range(M):
     A[y[j], j] = 1
 ```
```

### Comparing `lapx-0.5.8/setup.py` & `lapx-0.5.9/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,29 @@
-# # # # # # # # # # # # # # # # # # # # # #
-#    Rewrote on 2023/06/24 by rathaROG    #
-#    Updated on 2024/03/20 by rathaROG    #
-# # # # # # # # # # # # # # # # # # # # # #
-
+# Rewrote on 2023/06/24 by rathaROG
+# Updated on 2024/05/10 by rathaROG
 
 import distutils.cmd
-from setuptools import setup
-from setuptools.extension import Extension
-
-###################################################################
+from setuptools import Extension, setup
 
-DESCRIPTION = "Linear Assignment Problem solver (LAPJV/LAPMOD)."
 LICENSE = "BSD-2-Clause"
+DESCRIPTION = "Linear Assignment Problem solver (LAPJV/LAPMOD)."
 LONG_DESCRIPTION = open("README.md", encoding="utf-8").read()
 
-###################################################################
-
 package_name = "lapx"
 package_path = "lap"
 _lapjv_src = "_lapjv_src"
-requirements_txt = "requirements.txt"
-
-###################################################################
 
 def get_version_string():
     version_py = "lap/__init__.py"
     with open(version_py) as version_file:
         for line in version_file.read().splitlines():
             if line.startswith('__version__'):
                 delim = '"' if '"' in line else "'"
                 return line.split(delim)[1]
 
-def read_requirements():
-    with open(requirements_txt) as requirements_file:
-        return [line for line in requirements_file.read().splitlines()]
-
 def include_numpy():
     import numpy as np
     try:
         numpy_include = np.get_include()
     except AttributeError:
         numpy_include = np.get_numpy_include()
     return numpy_include
@@ -46,15 +31,15 @@
 def compile_cpp(cython_file):
     """Compile cpp from Cython's pyx or py.
     """
     import os
     import subprocess
     cpp_file = os.path.splitext(cython_file)[0] + ".cpp"
     flags = ['--fast-fail', '--cplus']
-    rc = subprocess.call(['cython'] + flags + ["-o", cpp_file, cython_file])
+    rc = subprocess.call(['cython'] + flags + ['-o', cpp_file, cython_file])
     if rc != 0: raise Exception('Cythonizing %s failed' % cython_file)
     else: return cpp_file
 
 class ExportCythonCommand(distutils.cmd.Command):
     description = "Export _lapjv binary from source."
     def run(self):
         super().run()
@@ -91,24 +76,24 @@
     packages = [package_path, tests_package]
     for p in packages: package_data.update({p: ["*"]})
 
     setup(
         name=package_name,
         version=get_version_string(),
         description=DESCRIPTION,
+        license=LICENSE,
         long_description=LONG_DESCRIPTION,
         long_description_content_type="text/markdown",
-        author="rathaROG",
+        keywords=['Linear Assignment', 'LAPJV', 'LAPMOD', 'lap'],
         url="https://github.com/rathaROG/lapx",
-        license=LICENSE,
+        author="rathaROG",
         packages=packages,
         package_data=package_data,
         include_package_data=True,
-        install_requires=read_requirements(),
-        keywords=['Linear Assignment', 'LAPJV', 'LAPMOD', 'lap'],
+        install_requires=['numpy>=1.21.6',],
         python_requires=">=3.7",
         classifiers=['Development Status :: 4 - Beta',
                      'Environment :: Console',
                      'Intended Audience :: Developers',
                      'Intended Audience :: Education',
                      'Intended Audience :: Science/Research',
                      'License :: OSI Approved :: BSD License',
```

