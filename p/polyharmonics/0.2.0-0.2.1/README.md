# Comparing `tmp/polyharmonics-0.2.0.tar.gz` & `tmp/polyharmonics-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyharmonics-0.2.0.tar", max compression
+gzip compressed data, was "polyharmonics-0.2.1.tar", max compression
```

## Comparing `polyharmonics-0.2.0.tar` & `polyharmonics-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rwxr-xr-x   0        0        0     1466 2024-04-16 13:33:46.000000 polyharmonics-0.2.0/LICENSE
--rwxr-xr-x   0        0        0     6137 2024-05-01 19:57:18.000000 polyharmonics-0.2.0/README.md
--rwxr-xr-x   0        0        0      459 2024-05-04 15:40:05.000000 polyharmonics-0.2.0/polyharmonics/__init__.py
--rwxr-xr-x   0        0        0     1075 2024-05-06 13:28:42.421280 polyharmonics-0.2.0/polyharmonics/__main__.py
--rwxr-xr-x   0        0        0     7241 2024-05-06 13:42:35.576924 polyharmonics-0.2.0/polyharmonics/associated_legendre_functions.py
--rwxr-xr-x   0        0        0      209 2024-05-06 13:28:42.418277 polyharmonics-0.2.0/polyharmonics/cli/__init__.py
--rwxr-xr-x   0        0        0     5707 2024-05-06 13:28:42.427725 polyharmonics-0.2.0/polyharmonics/cli/associated_legendre_cmd.py
--rwxr-xr-x   0        0        0      190 2024-05-06 13:28:42.418225 polyharmonics-0.2.0/polyharmonics/cli/benchmark/__init__.py
--rwxr-xr-x   0        0        0    13006 2024-05-06 13:41:16.581886 polyharmonics-0.2.0/polyharmonics/cli/benchmark/associated_legendre_bench.py
--rwxr-xr-x   0        0        0     5553 2024-05-06 13:41:16.580068 polyharmonics-0.2.0/polyharmonics/cli/benchmark/legendre_bench.py
--rwxr-xr-x   0        0        0      650 2024-05-06 13:28:42.421780 polyharmonics-0.2.0/polyharmonics/cli/benchmark_cmd.py
--rwxr-xr-x   0        0        0      183 2024-05-04 16:25:21.000000 polyharmonics-0.2.0/polyharmonics/cli/colors.py
--rwxr-xr-x   0        0        0     3456 2024-05-06 13:28:42.423962 polyharmonics-0.2.0/polyharmonics/cli/legendre_cmd.py
--rwxr-xr-x   0        0        0     4957 2024-05-06 13:37:17.743809 polyharmonics-0.2.0/polyharmonics/legendre_polynomials.py
--rwxr-xr-x   0        0        0     3462 2024-05-06 13:37:39.200763 polyharmonics-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7667 1970-01-01 00:00:00.000000 polyharmonics-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1466 2024-04-16 13:33:46.000000 polyharmonics-0.2.1/LICENSE
+-rwxr-xr-x   0        0        0     5766 2024-05-06 13:47:41.571445 polyharmonics-0.2.1/README.md
+-rwxr-xr-x   0        0        0      459 2024-05-04 15:40:05.000000 polyharmonics-0.2.1/polyharmonics/__init__.py
+-rwxr-xr-x   0        0        0     1075 2024-05-06 13:28:42.421280 polyharmonics-0.2.1/polyharmonics/__main__.py
+-rwxr-xr-x   0        0        0     7357 2024-05-10 19:01:36.870299 polyharmonics-0.2.1/polyharmonics/associated_legendre_functions.py
+-rwxr-xr-x   0        0        0      209 2024-05-06 13:28:42.418277 polyharmonics-0.2.1/polyharmonics/cli/__init__.py
+-rwxr-xr-x   0        0        0     5707 2024-05-06 13:28:42.427725 polyharmonics-0.2.1/polyharmonics/cli/associated_legendre_cmd.py
+-rwxr-xr-x   0        0        0      190 2024-05-06 13:28:42.418225 polyharmonics-0.2.1/polyharmonics/cli/benchmark/__init__.py
+-rwxr-xr-x   0        0        0    13006 2024-05-06 13:41:16.581886 polyharmonics-0.2.1/polyharmonics/cli/benchmark/associated_legendre_bench.py
+-rwxr-xr-x   0        0        0     5553 2024-05-06 13:41:16.580068 polyharmonics-0.2.1/polyharmonics/cli/benchmark/legendre_bench.py
+-rwxr-xr-x   0        0        0      650 2024-05-06 13:28:42.421780 polyharmonics-0.2.1/polyharmonics/cli/benchmark_cmd.py
+-rwxr-xr-x   0        0        0      183 2024-05-04 16:25:21.000000 polyharmonics-0.2.1/polyharmonics/cli/colors.py
+-rwxr-xr-x   0        0        0     3456 2024-05-06 13:28:42.423962 polyharmonics-0.2.1/polyharmonics/cli/legendre_cmd.py
+-rwxr-xr-x   0        0        0     4957 2024-05-06 13:37:17.743809 polyharmonics-0.2.1/polyharmonics/legendre_polynomials.py
+-rwxr-xr-x   0        0        0     3462 2024-05-10 18:59:45.448988 polyharmonics-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7296 1970-01-01 00:00:00.000000 polyharmonics-0.2.1/PKG-INFO
```

### Comparing `polyharmonics-0.2.0/LICENSE` & `polyharmonics-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polyharmonics-0.2.0/README.md` & `polyharmonics-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -144,39 +144,14 @@
 make check-codestyle && make test && make check-safety
 ```
 
 </p>
 </details>
 
 <details>
-<summary>Docker</summary>
-<p>
-
-```bash
-make docker-build
-```
-
-which is equivalent to:
-
-```bash
-make docker-build VERSION=latest
-```
-
-Remove docker image with
-
-```bash
-make docker-remove
-```
-
-More information [about docker](https://github.com/Undertone0809/python-package-template/tree/main/%7B%7B%20cookiecutter.project_name%20%7D%7D/docker).
-
-</p>
-</details>
-
-<details>
 <summary>Cleanup</summary>
 <p>
 Delete pycache files
 
 ```bash
 make pycache-remove
 ```
```

### Comparing `polyharmonics-0.2.0/polyharmonics/__main__.py` & `polyharmonics-0.2.1/polyharmonics/__main__.py`

 * *Files identical despite different names*

### Comparing `polyharmonics-0.2.0/polyharmonics/associated_legendre_functions.py` & `polyharmonics-0.2.1/polyharmonics/associated_legendre_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,20 @@
                     .subs((1 - x**2) ** Rational(1, 2), sin(th))
                     .subs(x, cos(th))
                 )
             else:
                 return ass_legendre_store.recursion[n][m]
         else:
             curr_fun, prev_fun = associated_legendre_rec(
-                n, m - 1, polar=False, store=store, callback=True
+                n,
+                m - 1,
+                polar=False,
+                store=store,
+                callback=True,
+                use_legendre_def=use_legendre_def,
             )
             fun: Expr = expand(
                 (
                     2 * (m - 1) * x * (1 - x**2) ** Rational(-1, 2) * curr_fun
                     - (n + m - 1) * (n - m + 2) * prev_fun
                 ),
                 deep=True,
```

### Comparing `polyharmonics-0.2.0/polyharmonics/cli/associated_legendre_cmd.py` & `polyharmonics-0.2.1/polyharmonics/cli/associated_legendre_cmd.py`

 * *Files identical despite different names*

### Comparing `polyharmonics-0.2.0/polyharmonics/cli/benchmark/associated_legendre_bench.py` & `polyharmonics-0.2.1/polyharmonics/cli/benchmark/associated_legendre_bench.py`

 * *Files identical despite different names*

### Comparing `polyharmonics-0.2.0/polyharmonics/cli/benchmark/legendre_bench.py` & `polyharmonics-0.2.1/polyharmonics/cli/benchmark/legendre_bench.py`

 * *Files identical despite different names*

### Comparing `polyharmonics-0.2.0/polyharmonics/cli/benchmark_cmd.py` & `polyharmonics-0.2.1/polyharmonics/cli/benchmark_cmd.py`

 * *Files identical despite different names*

### Comparing `polyharmonics-0.2.0/polyharmonics/cli/legendre_cmd.py` & `polyharmonics-0.2.1/polyharmonics/cli/legendre_cmd.py`

 * *Files identical despite different names*

### Comparing `polyharmonics-0.2.0/polyharmonics/legendre_polynomials.py` & `polyharmonics-0.2.1/polyharmonics/legendre_polynomials.py`

 * *Files identical despite different names*

### Comparing `polyharmonics-0.2.0/pyproject.toml` & `polyharmonics-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polyharmonics"
-version = "0.2.0"
+version = "0.2.1"
 description = "Ortogonal polynomials in the unit sphere"
 readme = "README.md"
 authors = [
   "Iván Salido Cobo <isalidocobo@gmail.com>",
 ]
 license = "BSD-3-Clause"
 repository = "https://github.com/ComicIvans/polyharmonics"
```

### Comparing `polyharmonics-0.2.0/PKG-INFO` & `polyharmonics-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyharmonics
-Version: 0.2.0
+Version: 0.2.1
 Summary: Ortogonal polynomials in the unit sphere
 Home-page: https://github.com/ComicIvans/polyharmonics
 License: BSD-3-Clause
 Keywords: python,polynomials,unit sphere,orthogonal polynomials,mathematics,math,legendre polynomials,associated legendre functions,spherical harmonics
 Author: Iván Salido Cobo
 Author-email: isalidocobo@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -177,39 +177,14 @@
 make check-codestyle && make test && make check-safety
 ```
 
 </p>
 </details>
 
 <details>
-<summary>Docker</summary>
-<p>
-
-```bash
-make docker-build
-```
-
-which is equivalent to:
-
-```bash
-make docker-build VERSION=latest
-```
-
-Remove docker image with
-
-```bash
-make docker-remove
-```
-
-More information [about docker](https://github.com/Undertone0809/python-package-template/tree/main/%7B%7B%20cookiecutter.project_name%20%7D%7D/docker).
-
-</p>
-</details>
-
-<details>
 <summary>Cleanup</summary>
 <p>
 Delete pycache files
 
 ```bash
 make pycache-remove
 ```
```

