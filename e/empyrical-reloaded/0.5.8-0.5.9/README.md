# Comparing `tmp/empyrical-reloaded-0.5.8.tar.gz` & `tmp/empyrical-reloaded-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empyrical-reloaded-0.5.8.tar", last modified: Sat Sep  4 21:27:39 2021, max compression
+gzip compressed data, was "empyrical-reloaded-0.5.9.tar", last modified: Tue Jan 10 22:30:49 2023, max compression
```

## Comparing `empyrical-reloaded-0.5.8.tar` & `empyrical-reloaded-0.5.9.tar`

### file list

```diff
@@ -1,23 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-04 21:27:39.110474 empyrical-reloaded-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11346 2021-09-04 21:27:27.000000 empyrical-reloaded-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-09-04 21:27:27.000000 empyrical-reloaded-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6258 2021-09-04 21:27:39.110474 empyrical-reloaded-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5298 2021-09-04 21:27:27.000000 empyrical-reloaded-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-04 21:27:39.110474 empyrical-reloaded-0.5.8/empyrical/
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2021-09-04 21:27:27.000000 empyrical-reloaded-0.5.8/empyrical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2021-09-04 21:27:39.110474 empyrical-reloaded-0.5.8/empyrical/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2021-09-04 21:27:27.000000 empyrical-reloaded-0.5.8/empyrical/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (121)     6009 2021-09-04 21:27:27.000000 empyrical-reloaded-0.5.8/empyrical/perf_attrib.py
--rw-r--r--   0 runner    (1001) docker     (121)      379 2021-09-04 21:27:27.000000 empyrical-reloaded-0.5.8/empyrical/periods.py
--rw-r--r--   0 runner    (1001) docker     (121)    66222 2021-09-04 21:27:27.000000 empyrical-reloaded-0.5.8/empyrical/stats.py
--rw-r--r--   0 runner    (1001) docker     (121)    15325 2021-09-04 21:27:27.000000 empyrical-reloaded-0.5.8/empyrical/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-04 21:27:39.110474 empyrical-reloaded-0.5.8/empyrical_reloaded.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6258 2021-09-04 21:27:39.000000 empyrical-reloaded-0.5.8/empyrical_reloaded.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      437 2021-09-04 21:27:39.000000 empyrical-reloaded-0.5.8/empyrical_reloaded.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-04 21:27:39.000000 empyrical-reloaded-0.5.8/empyrical_reloaded.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      606 2021-09-04 21:27:39.000000 empyrical-reloaded-0.5.8/empyrical_reloaded.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-09-04 21:27:39.000000 empyrical-reloaded-0.5.8/empyrical_reloaded.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      338 2021-09-04 21:27:27.000000 empyrical-reloaded-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2021-09-04 21:27:39.110474 empyrical-reloaded-0.5.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1123 2021-09-04 21:27:27.000000 empyrical-reloaded-0.5.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    65984 2021-09-04 21:27:27.000000 empyrical-reloaded-0.5.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:30:49.893396 empyrical-reloaded-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:30:49.889396 empyrical-reloaded-0.5.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:30:49.889396 empyrical-reloaded-0.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/.github/workflows/build_wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/.github/workflows/ci_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/.github/workflows/conda_package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/.github/workflows/test_wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/.github/workflows/unit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19417 2023-01-10 22:30:49.893396 empyrical-reloaded-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:30:49.889396 empyrical-reloaded-0.5.9/conda/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:30:49.889396 empyrical-reloaded-0.5.9/conda/recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/conda/recipe/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:30:49.889396 empyrical-reloaded-0.5.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/docs/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/docs/make_docs.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:30:49.893396 empyrical-reloaded-0.5.9/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/docs/source/perf_attrib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/docs/source/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/docs/source/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-10 22:30:49.893396 empyrical-reloaded-0.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:30:49.889396 empyrical-reloaded-0.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:30:49.893396 empyrical-reloaded-0.5.9/src/empyrical/
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/src/empyrical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-10 22:30:49.000000 empyrical-reloaded-0.5.9/src/empyrical/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/src/empyrical/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/src/empyrical/perf_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/src/empyrical/periods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63704 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/src/empyrical/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/src/empyrical/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:30:49.893396 empyrical-reloaded-0.5.9/src/empyrical_reloaded.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19417 2023-01-10 22:30:49.000000 empyrical-reloaded-0.5.9/src/empyrical_reloaded.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-01-10 22:30:49.000000 empyrical-reloaded-0.5.9/src/empyrical_reloaded.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 22:30:49.000000 empyrical-reloaded-0.5.9/src/empyrical_reloaded.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 22:30:49.000000 empyrical-reloaded-0.5.9/src/empyrical_reloaded.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-01-10 22:30:49.000000 empyrical-reloaded-0.5.9/src/empyrical_reloaded.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-10 22:30:49.000000 empyrical-reloaded-0.5.9/src/empyrical_reloaded.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:30:49.893396 empyrical-reloaded-0.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10107 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:30:49.893396 empyrical-reloaded-0.5.9/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    25231 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/tests/test_data/factor_loadings.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/tests/test_data/factor_returns.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/tests/test_data/intercepts.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/tests/test_data/positions.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/tests/test_data/residuals.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/tests/test_data/returns.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/tests/test_perf_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67633 2023-01-10 22:30:37.000000 empyrical-reloaded-0.5.9/tests/test_stats.py
```

### Comparing `empyrical-reloaded-0.5.8/LICENSE` & `empyrical-reloaded-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `empyrical-reloaded-0.5.8/PKG-INFO` & `empyrical-reloaded-0.5.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: empyrical-reloaded
-Version: 0.5.8
-Summary: empyrical computes performance and risk statistics commonly used in quantitative finance
-Home-page: https://empyrical.ml4trading.io
-Author: Quantopian Inc
-Maintainer: Applied AI, LLC
-License: Apache 2.0
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: doc
-License-File: LICENSE
-
 <p align="center">
 <a href="https://empyrical.ml4trading.io">
 <img src="https://i.imgur.com/PbZNeud.png" width="35%">
 </a>
 </p>
 
 ![PyPI](https://img.shields.io/pypi/v/empyrical-reloaded)
@@ -185,9 +158,7 @@
 
 - install requirements
     - "pytest>=6.2.0",
 
 ```bash
 pytest tests
 ```
-
-
```

#### html2text {}

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1 Name: empyrical-reloaded Version: 0.5.8 Summary:
-empyrical computes performance and risk statistics commonly used in
-quantitative finance Home-page: https://empyrical.ml4trading.io Author:
-Quantopian Inc Maintainer: Applied AI, LLC License: Apache 2.0 Platform:
-UNKNOWN Classifier: Development Status :: 4 - Beta Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Intended Audience :: Science/Research Classifier:
-Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
-Mathematics Classifier: Operating System :: OS Independent Requires-Python:
->=3.7 Description-Content-Type: text/markdown Provides-Extra: all Provides-
-Extra: test Provides-Extra: dev Provides-Extra: doc License-File: LICENSE
                        _[_h_t_t_p_s_:_/_/_i_._i_m_g_u_r_._c_o_m_/_P_b_Z_N_e_u_d_._p_n_g_]
 ![PyPI](https://img.shields.io/pypi/v/empyrical-reloaded) ![Conda (channel
 only)](https://img.shields.io/conda/vn/ml4t/empyrical-reloaded) [![PyPI Wheels]
 (https://github.com/stefan-jansen/empyrical-reloaded/actions/workflows/
 build_wheels.yml/badge.svg)](https://github.com/stefan-jansen/empyrical-
 reloaded/actions/workflows/build_wheels.yml) [![Conda packages](https://
 github.com/stefan-jansen/empyrical-reloaded/actions/workflows/
```

### Comparing `empyrical-reloaded-0.5.8/empyrical/__init__.py` & `empyrical-reloaded-0.5.9/src/empyrical/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # flake8: noqa
 
-from ._version import get_versions
-
-__version__ = get_versions()["version"]
-del get_versions
+try:
+    from ._version import version as __version__
+    from ._version import version_tuple
+except ImportError:
+    __version__ = "unknown version"
+    version_tuple = (0, 0, "unknown version")
 
 from .stats import (
     aggregate_returns,
     alpha,
     alpha_aligned,
     alpha_beta,
     alpha_beta_aligned,
@@ -44,15 +46,14 @@
     downside_risk,
     excess_sharpe,
     max_drawdown,
     omega_ratio,
     roll_alpha,
     roll_alpha_aligned,
     roll_alpha_beta,
-    roll_alpha_beta,
     roll_alpha_beta_aligned,
     roll_annual_volatility,
     roll_beta,
     roll_beta_aligned,
     roll_down_capture,
     roll_max_drawdown,
     roll_sharpe_ratio,
@@ -63,14 +64,15 @@
     simple_returns,
     sortino_ratio,
     stability_of_timeseries,
     tail_ratio,
     up_alpha_beta,
     up_capture,
     up_down_capture,
+    batting_average,
     value_at_risk,
 )
 
 from .periods import DAILY, WEEKLY, MONTHLY, QUARTERLY, YEARLY
 
 
 from .perf_attrib import (
```

### Comparing `empyrical-reloaded-0.5.8/empyrical/deprecate.py` & `empyrical-reloaded-0.5.9/src/empyrical/deprecate.py`

 * *Files identical despite different names*

### Comparing `empyrical-reloaded-0.5.8/empyrical/perf_attrib.py` & `empyrical-reloaded-0.5.9/src/empyrical/perf_attrib.py`

 * *Files identical despite different names*

### Comparing `empyrical-reloaded-0.5.8/empyrical/stats.py` & `empyrical-reloaded-0.5.9/src/empyrical/stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,145 +10,43 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import math
-import pandas as pd
-import numpy as np
+from collections import OrderedDict
 from math import pow
-from scipy import stats, optimize
 from sys import float_info
 
-from .utils import nanmean, nanstd, nanmin, up, down, roll, rolling_window
-from .periods import ANNUALIZATION_FACTORS, APPROX_BDAYS_PER_YEAR
-from .periods import DAILY, WEEKLY, MONTHLY, QUARTERLY, YEARLY
-
-
-def _create_unary_vectorized_roll_function(function):
-    def unary_vectorized_roll(arr, window, out=None, **kwargs):
-        """
-        Computes the {human_readable} measure over a rolling window.
-
-        Parameters
-        ----------
-        arr : array-like
-            The array to compute the rolling {human_readable} over.
-        window : int
-            Size of the rolling window in terms of the periodicity of the data.
-        out : array-like, optional
-            Array to use as output buffer.
-            If not passed, a new array will be created.
-        **kwargs
-            Forwarded to :func:`~empyrical.{name}`.
-
-        Returns
-        -------
-        rolling_{name} : array-like
-            The rolling {human_readable}.
-        """
-        allocated_output = out is None
-
-        if len(arr):
-            out = function(
-                rolling_window(_flatten(arr), min(len(arr), window)).T,
-                out=out,
-                **kwargs,
-            )
-        else:
-            out = np.empty(0, dtype="float64")
-
-        if allocated_output and isinstance(arr, pd.Series):
-            out = pd.Series(out, index=arr.index[-len(out) :])
-
-        return out
-
-    unary_vectorized_roll.__doc__ = unary_vectorized_roll.__doc__.format(
-        name=function.__name__,
-        human_readable=function.__name__.replace("_", " "),
-    )
-
-    return unary_vectorized_roll
-
-
-def _create_binary_vectorized_roll_function(function):
-    def binary_vectorized_roll(lhs, rhs, window, out=None, **kwargs):
-        """
-        Computes the {human_readable} measure over a rolling window.
-
-        Parameters
-        ----------
-        lhs : array-like
-            The first array to pass to the rolling {human_readable}.
-        rhs : array-like
-            The second array to pass to the rolling {human_readable}.
-        window : int
-            Size of the rolling window in terms of the periodicity of the data.
-        out : array-like, optional
-            Array to use as output buffer.
-            If not passed, a new array will be created.
-        **kwargs
-            Forwarded to :func:`~empyrical.{name}`.
-
-        Returns
-        -------
-        rolling_{name} : array-like
-            The rolling {human_readable}.
-        """
-        allocated_output = out is None
-
-        if window >= 1 and len(lhs) and len(rhs):
-            out = function(
-                rolling_window(_flatten(lhs), min(len(lhs), window)).T,
-                rolling_window(_flatten(rhs), min(len(rhs), window)).T,
-                out=out,
-                **kwargs,
-            )
-        elif allocated_output:
-            out = np.empty(0, dtype="float64")
-        else:
-            out[()] = np.nan
-
-        if allocated_output:
-            if out.ndim == 1 and isinstance(lhs, pd.Series):
-                out = pd.Series(out, index=lhs.index[-len(out) :])
-            elif out.ndim == 2 and isinstance(lhs, pd.Series):
-                out = pd.DataFrame(out, index=lhs.index[-len(out) :])
-        return out
-
-    binary_vectorized_roll.__doc__ = binary_vectorized_roll.__doc__.format(
-        name=function.__name__,
-        human_readable=function.__name__.replace("_", " "),
-    )
-
-    return binary_vectorized_roll
-
-
-def _flatten(arr):
-    return arr if not isinstance(arr, pd.Series) else arr.values
-
-
-def _adjust_returns(returns, adjustment_factor):
-    """
-    Returns the returns series adjusted by adjustment_factor. Optimizes for the
-    case of adjustment_factor being 0 by returning returns itself, not a copy!
-
-    Parameters
-    ----------
-    returns : pd.Series or np.ndarray
-    adjustment_factor : pd.Series or np.ndarray or float or int
+import numpy as np
+import pandas as pd
+from scipy import optimize, stats
 
-    Returns
-    -------
-    adjusted_returns : array-like
-    """
-    if isinstance(adjustment_factor, (float, int)) and adjustment_factor == 0:
-        return returns
-    return returns - adjustment_factor
+from .periods import (
+    ANNUALIZATION_FACTORS,
+    APPROX_BDAYS_PER_YEAR,
+    DAILY,
+    MONTHLY,
+    QUARTERLY,
+    WEEKLY,
+    YEARLY,
+)
+from .utils import (
+    _adjust_returns,
+    _aligned_series,
+    _create_binary_vectorized_roll_function,
+    _create_unary_vectorized_roll_function,
+    down,
+    nanmean,
+    nanmin,
+    nanstd,
+    roll,
+    up,
+)
 
 
 def annualization_factor(period, annualization):
     """
     Return annualization factor from period entered or if a custom
     value is passed in.
 
@@ -174,17 +72,15 @@
     """
     if annualization is None:
         try:
             factor = ANNUALIZATION_FACTORS[period]
         except KeyError:
             raise ValueError(
                 "Period cannot be '{}'. "
-                "Can be '{}'.".format(
-                    period, "', '".join(ANNUALIZATION_FACTORS.keys())
-                )
+                "Can be '{}'.".format(period, "', '".join(ANNUALIZATION_FACTORS.keys()))
             )
     else:
         factor = annualization
     return factor
 
 
 def simple_returns(prices):
@@ -204,15 +100,18 @@
         and index coerced to be tz-aware.
     """
     if isinstance(prices, (pd.DataFrame, pd.Series)):
         out = prices.pct_change().iloc[1:]
     else:
         # Assume np.ndarray
         out = np.diff(prices, axis=0)
-        np.divide(out, prices[:-1], out=out)
+
+        # Silence divide error warnings
+        with np.errstate(divide="ignore", invalid="ignore"):
+            np.divide(out, prices[:-1], out=out)
 
     return out
 
 
 def cum_returns(returns, starting_value=0, out=None):
     """
     Compute cumulative returns from simple returns.
@@ -344,63 +243,109 @@
         raise ValueError(
             "convert_to must be {}, {} or {}".format(WEEKLY, MONTHLY, YEARLY)
         )
 
     return returns.groupby(grouping).apply(cumulate_returns)
 
 
-def max_drawdown(returns, out=None):
+def drawdown_series(returns, out=None):
     """
-    Determines the maximum drawdown of a strategy.
+    Computes the series of drawdowns of a strategy.
 
     Parameters
     ----------
-    returns : pd.Series or np.ndarray
+    returns : pd.Series, pd.DataFrame or np.ndarray
         Daily returns of the strategy, noncumulative.
         - See full explanation in :func:`~empyrical.stats.cum_returns`.
     out : array-like, optional
         Array to use as output buffer.
         If not passed, a new array will be created.
 
     Returns
     -------
-    max_drawdown : float
+    drawdown_series :  pd.Series, pd.DataFrame or np.ndarray
 
     Note
     -----
     See https://en.wikipedia.org/wiki/Drawdown_(economics) for more details.
     """
     allocated_output = out is None
     if allocated_output:
-        out = np.empty(returns.shape[1:])
+        out = np.empty(
+            (returns.shape[0] + 1,) + returns.shape[1:],
+            dtype="float64",
+        )
 
     returns_1d = returns.ndim == 1
 
     if len(returns) < 1:
         out[()] = np.nan
         if returns_1d:
             out = out.item()
         return out
 
     returns_array = np.asanyarray(returns)
 
-    cumulative = np.empty(
-        (returns.shape[0] + 1,) + returns.shape[1:],
-        dtype="float64",
-    )
-    cumulative[0] = start = 100
-    cum_returns(returns_array, starting_value=start, out=cumulative[1:])
+    out[0] = start = 100
+    cum_returns(returns_array, starting_value=start, out=out[1:])
+
+    max_return = np.fmax.accumulate(out, axis=0)
+
+    np.divide((out - max_return), max_return, out=out)
+
+    if returns.ndim == 1 and isinstance(returns, pd.Series):
+        out = pd.Series(out[1:], index=returns.index)
+    elif isinstance(returns, pd.DataFrame):
+        out = pd.DataFrame(
+            out[1:],
+            index=returns.index,
+            columns=returns.columns,
+        )
+
+    return out
+
+
+def max_drawdown(returns, out=None):
+    """
+    Determines the maximum drawdown of a strategy.
+
+    Parameters
+    ----------
+    returns : pd.Series or np.ndarray
+        Daily returns of the strategy, noncumulative.
+        - See full explanation in :func:`~empyrical.stats.cum_returns`.
+    out : array-like, optional
+        Array to use as output buffer.
+        If not passed, a new array will be created.
+
+    Returns
+    -------
+    max_drawdown : float, np.array or pd.Series
+
+    Note
+    -----
+    See https://en.wikipedia.org/wiki/Drawdown_(economics) for more details.
+    """
+    allocated_output = out is None
+    if allocated_output:
+        out = np.empty(returns.shape[1:])
+
+    returns_1d = returns.ndim == 1
 
-    max_return = np.fmax.accumulate(cumulative, axis=0)
+    if len(returns) < 1:
+        out[()] = np.nan
+        if returns_1d:
+            out = out.item()
+        return out
 
-    nanmin((cumulative - max_return) / max_return, axis=0, out=out)
+    nanmin(drawdown_series(returns), axis=0, out=out)
     if returns_1d:
         out = out.item()
     elif allocated_output and isinstance(returns, pd.DataFrame):
-        out = pd.Series(out)
+        out = pd.Series(out, index=returns.columns)
 
     return out
 
 
 roll_max_drawdown = _create_unary_vectorized_roll_function(max_drawdown)
 
 
@@ -479,17 +424,15 @@
     """
     return annual_return(returns, period, annualization)
 
 
 roll_cagr = _create_unary_vectorized_roll_function(cagr)
 
 
-def annual_volatility(
-    returns, period=DAILY, alpha=2.0, annualization=None, out=None
-):
+def annual_volatility(returns, period=DAILY, alpha=2.0, annualization=None, out=None):
     """
     Determines the annual volatility of a strategy.
 
     Parameters
     ----------
     returns : pd.Series or np.ndarray
         Periodic returns of the strategy, noncumulative.
@@ -643,17 +586,15 @@
 
     if denom > 0.0:
         return numer / denom
     else:
         return np.nan
 
 
-def sharpe_ratio(
-    returns, risk_free=0, period=DAILY, annualization=None, out=None
-):
+def sharpe_ratio(returns, risk_free=0, period=DAILY, annualization=None, out=None):
     """
     Determines the Sharpe ratio of a strategy.
 
     Parameters
     ----------
     returns : pd.Series or np.ndarray
         Daily returns of the strategy, noncumulative.
@@ -698,23 +639,26 @@
         if return_1d:
             out = out.item()
         return out
 
     returns_risk_adj = np.asanyarray(_adjust_returns(returns, risk_free))
     ann_factor = annualization_factor(period, annualization)
 
-    np.multiply(
-        np.divide(
-            nanmean(returns_risk_adj, axis=0),
-            nanstd(returns_risk_adj, ddof=1, axis=0),
+    # Silence divide error warnings
+    with np.errstate(divide="ignore", invalid="ignore"):
+        np.multiply(
+            np.divide(
+                nanmean(returns_risk_adj, axis=0),
+                nanstd(returns_risk_adj, ddof=1, axis=0),
+                out=out,
+            ),
+            np.sqrt(ann_factor),
             out=out,
-        ),
-        np.sqrt(ann_factor),
-        out=out,
-    )
+        )
+
     if return_1d:
         out = out.item()
 
     return out
 
 
 roll_sharpe_ratio = _create_unary_vectorized_roll_function(sharpe_ratio)
@@ -790,15 +734,19 @@
 
     average_annual_return = nanmean(adj_returns, axis=0) * ann_factor
     annualized_downside_risk = (
         _downside_risk
         if _downside_risk is not None
         else downside_risk(returns, required_return, period, annualization)
     )
-    np.divide(average_annual_return, annualized_downside_risk, out=out)
+
+    # Silence divide error warnings
+    with np.errstate(divide="ignore", invalid="ignore"):
+        np.divide(average_annual_return, annualized_downside_risk, out=out)
+
     if return_1d:
         out = out.item()
     elif isinstance(returns, pd.DataFrame):
         out = pd.Series(out)
 
     return out
 
@@ -922,85 +870,30 @@
         if returns_1d:
             out = out.item()
         return out
 
     active_return = _adjust_returns(returns, factor_returns)
     tracking_error = np.nan_to_num(nanstd(active_return, ddof=1, axis=0))
 
-    out = np.divide(
-        nanmean(active_return, axis=0, out=out),
-        tracking_error,
-        out=out,
-    )
+    # Silence divide warnings
+    with np.errstate(divide="ignore", invalid="ignore"):
+        out = np.divide(
+            nanmean(active_return, axis=0, out=out),
+            tracking_error,
+            out=out,
+        )
+
     if returns_1d:
         out = out.item()
     return out
 
 
 roll_excess_sharpe = _create_binary_vectorized_roll_function(excess_sharpe)
 
 
-def _to_pandas(ob):
-    """Convert an array-like to a pandas object.
-
-    Parameters
-    ----------
-    ob : array-like
-        The object to convert.
-
-    Returns
-    -------
-    pandas_structure : pd.Series or pd.DataFrame
-        The correct structure based on the dimensionality of the data.
-    """
-    if isinstance(ob, (pd.Series, pd.DataFrame)):
-        return ob
-
-    if ob.ndim == 1:
-        return pd.Series(ob)
-    elif ob.ndim == 2:
-        return pd.DataFrame(ob)
-    else:
-        raise ValueError(
-            "cannot convert array of dim > 2 to a pandas structure",
-        )
-
-
-def _aligned_series(*many_series):
-    """
-    Return a new list of series containing the data in the input series, but
-    with their indices aligned. NaNs will be filled in for missing values.
-
-    Parameters
-    ----------
-    *many_series
-        The series to align.
-
-    Returns
-    -------
-    aligned_series : iterable[array-like]
-        A new list of series containing the data in the input series, but
-        with their indices aligned. NaNs will be filled in for missing values.
-
-    """
-    head = many_series[0]
-    tail = many_series[1:]
-    n = len(head)
-    if isinstance(head, np.ndarray) and all(
-        len(s) == n and isinstance(s, np.ndarray) for s in tail
-    ):
-        # optimization: ndarrays of the same length are already aligned
-        return many_series
-
-    # dataframe has no ``itervalues``
-    return (
-        v for _, v in pd.concat(map(_to_pandas, many_series), axis=1).items()
-    )
-
-
 def alpha_beta(
     returns,
     factor_returns,
     risk_free=0.0,
     period=DAILY,
     annualization=None,
     out=None,
@@ -1069,17 +962,15 @@
         Array to use as output buffer.
         If not passed, a new array will be created.
     **kwargs
         Forwarded to :func:`~empyrical.alpha_beta`.
     """
     returns, factor_returns = _aligned_series(returns, factor_returns)
 
-    return roll_alpha_beta_aligned(
-        returns, factor_returns, window=window, **kwargs
-    )
+    return roll_alpha_beta_aligned(returns, factor_returns, window=window, **kwargs)
 
 
 def alpha_beta_aligned(
     returns,
     factor_returns,
     risk_free=0.0,
     period=DAILY,
@@ -1193,18 +1084,15 @@
         If not passed, a new array will be created.
 
     Returns
     -------
     float
         Alpha.
     """
-    if not (
-        isinstance(returns, np.ndarray)
-        and isinstance(factor_returns, np.ndarray)
-    ):
+    if not (isinstance(returns, np.ndarray) and isinstance(factor_returns, np.ndarray)):
         returns, factor_returns = _aligned_series(returns, factor_returns)
 
     return alpha_aligned(
         returns,
         factor_returns,
         risk_free=risk_free,
         period=period,
@@ -1329,18 +1217,15 @@
         Array to use as output buffer.
         If not passed, a new array will be created.
 
     Returns
     -------
     beta : float
     """
-    if not (
-        isinstance(returns, np.ndarray)
-        and isinstance(factor_returns, np.ndarray)
-    ):
+    if not (isinstance(returns, np.ndarray) and isinstance(factor_returns, np.ndarray)):
         returns, factor_returns = _aligned_series(returns, factor_returns)
 
     return beta_aligned(
         returns,
         factor_returns,
         risk_free=risk_free,
         out=out,
@@ -1489,19 +1374,17 @@
     if len(returns) < 2:
         return np.nan
 
     returns = np.asanyarray(returns)
     returns = returns[~np.isnan(returns)]
 
     cum_log_returns = np.log1p(returns).cumsum()
-    rhat = stats.linregress(np.arange(len(cum_log_returns)), cum_log_returns)[
-        2
-    ]
+    rhat = stats.linregress(np.arange(len(cum_log_returns)), cum_log_returns)[2]
 
-    return rhat ** 2
+    return rhat**2
 
 
 def tail_ratio(returns):
     """Determines the ratio between the right (95%) and left tail (5%).
 
     For example, a ratio of 0.25 means that losses are four times
     as bad as profits.
@@ -1522,17 +1405,15 @@
 
     returns = np.asanyarray(returns)
     # Be tolerant of nan's
     returns = returns[~np.isnan(returns)]
     if len(returns) < 1:
         return np.nan
 
-    return np.abs(np.percentile(returns, 95)) / np.abs(
-        np.percentile(returns, 5)
-    )
+    return np.abs(np.percentile(returns, 95)) / np.abs(np.percentile(returns, 5))
 
 
 def capture(returns, factor_returns, period=DAILY):
     """Compute capture ratio.
 
     Parameters
     ----------
@@ -1595,17 +1476,15 @@
     Tail Risks: Application to Stress Testing`
             https://www.imf.org/external/pubs/ft/wp/2012/wp12216.pdf
             An IMF Working Paper describing the heuristic
     """
     if len(returns) < 3 or len(factor_returns) < 3:
         return np.nan
 
-    return beta_fragility_heuristic_aligned(
-        *_aligned_series(returns, factor_returns)
-    )
+    return beta_fragility_heuristic_aligned(*_aligned_series(returns, factor_returns))
 
 
 def beta_fragility_heuristic_aligned(returns, factor_returns):
     """Estimate fragility to drops in beta
 
         Parameters
         ----------
@@ -1766,17 +1645,15 @@
         losses = flipped_returns[flipped_returns > 0]
         threshold = DEFAULT_THRESHOLD
         finished = False
         scale_param = 0
         shape_param = 0
         while not finished and threshold > MINIMUM_THRESHOLD:
             losses_beyond_threshold = losses[losses >= threshold]
-            param_result = gpd_loglikelihood_minimizer_aligned(
-                losses_beyond_threshold
-            )
+            param_result = gpd_loglikelihood_minimizer_aligned(losses_beyond_threshold)
             if param_result[0] is not False and param_result[1] is not False:
                 scale_param = param_result[0]
                 shape_param = param_result[1]
                 var_estimate = gpd_var_calculator(
                     threshold,
                     scale_param,
                     shape_param,
@@ -1809,32 +1686,28 @@
 
 
 def gpd_es_calculator(var_estimate, threshold, scale_param, shape_param):
     result = 0
     if (1 - shape_param) != 0:
         # this formula is from Gilli and Kellezi pg. 8
         var_ratio = var_estimate / (1 - shape_param)
-        param_ratio = (scale_param - (shape_param * threshold)) / (
-            1 - shape_param
-        )
+        param_ratio = (scale_param - (shape_param * threshold)) / (1 - shape_param)
         result = var_ratio + param_ratio
     return result
 
 
 def gpd_var_calculator(
     threshold, scale_param, shape_param, probability, total_n, exceedance_n
 ):
     result = 0
     if exceedance_n > 0 and shape_param > 0:
         # this formula is from Gilli and Kellezi pg. 12
         param_ratio = scale_param / shape_param
         prob_ratio = (total_n / exceedance_n) * probability
-        result = threshold + (
-            param_ratio * (pow(prob_ratio, -shape_param) - 1)
-        )
+        result = threshold + (param_ratio * (pow(prob_ratio, -shape_param) - 1))
     return result
 
 
 def gpd_loglikelihood_minimizer_aligned(price_data):
     result = [False, False]
     DEFAULT_SCALE_PARAM = 1
     DEFAULT_SHAPE_PARAM = 1
@@ -1855,17 +1728,15 @@
 
 def gpd_loglikelihood_factory(price_data):
     return lambda params: gpd_loglikelihood(params, price_data)
 
 
 def gpd_loglikelihood(params, price_data):
     if params[1] != 0:
-        return -gpd_loglikelihood_scale_and_shape(
-            params[0], params[1], price_data
-        )
+        return -gpd_loglikelihood_scale_and_shape(params[0], params[1], price_data)
     else:
         return -gpd_loglikelihood_scale_only(params[0], price_data)
 
 
 def gpd_loglikelihood_scale_and_shape_factory(price_data):
     # minimize a function of two variables requires a list of params
     # we are expecting the lambda below to be called as follows:
@@ -1879,16 +1750,15 @@
 def gpd_loglikelihood_scale_and_shape(scale, shape, price_data):
     n = len(price_data)
     result = -1 * float_info.max
     if scale != 0:
         param_factor = shape / scale
         if shape != 0 and param_factor >= 0 and scale >= 0:
             result = (-n * np.log(scale)) - (
-                ((1 / shape) + 1)
-                * (np.log((shape / scale * price_data) + 1)).sum()
+                ((1 / shape) + 1) * (np.log((shape / scale * price_data) + 1)).sum()
             )
     return result
 
 
 def gpd_loglikelihood_scale_only_factory(price_data):
     # the negative is added because scipy only minimizes
     return lambda scale: -gpd_loglikelihood_scale_only(scale, price_data)
@@ -1999,14 +1869,56 @@
         the updown capture ratio
     """
     return up_capture(returns, factor_returns, **kwargs) / down_capture(
         returns, factor_returns, **kwargs
     )
 
 
+def batting_average(returns, factor_returns):
+    """
+    Computes the batting average.
+    Parameters
+    ----------
+    returns : pd.Series or np.ndarray
+        Returns of the strategy, noncumulative.
+        - See full explanation in :func:`~empyrical.stats.cum_returns`.
+    factor_returns : pd.Series or np.ndarray
+        Noncumulative returns of the factor to which beta is
+        computed. Usually a benchmark such as the market.
+        - This is in the same style as returns.
+    Returns
+    -------
+    batting_average : pd.Series
+        batting average, up market, down market
+    Note
+    ----
+    See https://www.investopedia.com/terms/b/batting-average.asp for
+    more information.
+    """
+    results = OrderedDict(
+        {
+            "batting average": np.nan,
+            "up market": np.nan,
+            "down market": np.nan,
+        }
+    )
+    active_return = _adjust_returns(returns, factor_returns)
+    bt = active_return > 0
+    up = active_return[factor_returns >= 0.0] > 0
+    down = active_return[factor_returns < 0.0] > 0
+    if len(bt) > 0:
+        results["batting average"] = bt.mean()
+    if len(up) > 0:
+        results["up market"] = up.mean()
+    if len(down) > 0:
+        results["down market"] = down.mean()
+
+    return pd.Series(results, index=results.keys())
+
+
 def up_alpha_beta(returns, factor_returns, **kwargs):
     """
     Computes alpha and beta for periods when the benchmark return is positive.
 
     Parameters
     ----------
     see documentation for `alpha_beta`.
@@ -2054,17 +1966,15 @@
         computed. Usually a benchmark such as the market.
         - This is in the same style as returns.
 
     window : int, required
         Size of the rolling window in terms of the periodicity of the data.
         - eg window = 60, periodicity=DAILY, represents a rolling 60 day window
     """
-    return roll(
-        returns, factor_returns, window=window, function=up_capture, **kwargs
-    )
+    return roll(returns, factor_returns, window=window, function=up_capture, **kwargs)
 
 
 def roll_down_capture(returns, factor_returns, window=10, **kwargs):
     """
     Computes the down capture measure over a rolling window.
     see documentation for :func:`~empyrical.stats.down_capture`.
     (pass all args, kwargs required)
@@ -2080,17 +1990,15 @@
         computed. Usually a benchmark such as the market.
         - This is in the same style as returns.
 
     window : int, required
         Size of the rolling window in terms of the periodicity of the data.
         - eg window = 60, periodicity=DAILY, represents a rolling 60 day window
     """
-    return roll(
-        returns, factor_returns, window=window, function=down_capture, **kwargs
-    )
+    return roll(returns, factor_returns, window=window, function=down_capture, **kwargs)
 
 
 def roll_up_down_capture(returns, factor_returns, window=10, **kwargs):
     """
     Computes the up/down capture measure over a rolling window.
     see documentation for :func:`~empyrical.stats.up_down_capture`.
     (pass all args, kwargs required)
```

### Comparing `empyrical-reloaded-0.5.8/empyrical/utils.py` & `empyrical-reloaded-0.5.9/src/empyrical/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import errno
+import warnings
 from datetime import datetime
-from functools import wraps
+from functools import wraps, partial
 from os import makedirs, environ
 from os.path import expanduser, join, getmtime, isdir
-import errno
-import warnings
 
 import numpy as np
-from numpy.lib.stride_tricks import as_strided
 import pandas as pd
+import yfinance as yf
+from numpy.lib.stride_tricks import as_strided
 from pandas.tseries.offsets import BDay
 from pandas_datareader import data as web
-import yfinance as yf
+from pytz import UTC
 
 try:
     # fast versions
     import bottleneck as bn
 
     def _wrap_function(f):
         @wraps(f)
@@ -236,41 +237,51 @@
 _1_bday = BDay()
 
 
 def _1_bday_ago():
     return pd.Timestamp.now().normalize() - _1_bday
 
 
-# ToDo: start & end parameters; choose FF data
-def get_fama_french():
+def get_fama_french(
+    start="1-1-1970",
+    end=None,
+    datasets=[
+        "F-F_Research_Data_Factors_daily",
+        "F-F_Momentum_Factor_daily",
+    ],
+):
     """
     Retrieve Fama-French factors via pandas-datareader
+    Parameters
+    ----------
+    start: str or datetime or Timestamp, start date
+    end: str or datetime or Timestamp, end date
+    datasets: list of factors (default is the five factors)
     Returns
     -------
     pandas.DataFrame
         Percent change of Fama-French factors
     """
-
-    start = "1/1/1970"
-    research_factors = web.DataReader(
-        "F-F_Research_Data_Factors_daily", "famafrench", start=start
-    )[0]
-
-    momentum_factor = web.DataReader(
-        "F-F_Momentum_Factor_daily", "famafrench", start=start
-    )[0]
-
-    five_factors = (
-        research_factors.join(momentum_factor)
-        .dropna()
-        .div(100)
-        .rename(columns=str.strip)
+    if not isinstance(start, datetime):
+        start = pd.Timestamp(start).date()
+    if not isinstance(end, datetime):
+        end = pd.Timestamp(end).date()
+
+    ff_function = partial(
+        web.DataReader,
+        data_source="famafrench",
+        start=start,
+        end=end,
     )
-    five_factors.index = five_factors.index.tz_localize("utc")
-    return five_factors
+
+    df = [ff_function(dataset)[0] for dataset in datasets]
+    df = pd.concat(df, axis=1).dropna().div(100).rename(columns=str.strip)
+
+    df.index = df.index.tz_localize("utc")
+    return df
 
 
 def get_returns_cached(filepath, update_func, latest_dt, **kwargs):
     """
     Get returns from a cached file if the cache is recent enough,
     otherwise, try to retrieve via a provided update function and
     update the cache file.
@@ -305,15 +316,16 @@
         if latest_dt.tzinfo:
             file_dt = file_dt.tz_localize("utc")
 
         if file_dt < latest_dt:
             update_cache = True
         else:
             returns = pd.read_csv(filepath, index_col=0, parse_dates=True)
-            returns.index = returns.index.tz_localize("UTC")
+            if returns.index.tz != UTC:
+                returns.index = returns.index.tz_localize("UTC")
 
     if update_cache:
         returns = update_func(**kwargs)
         try:
             ensure_directory(cache_dir())
         except OSError as e:
             warnings.warn(
@@ -390,17 +402,15 @@
     """
 
     if start is None:
         start = "1970-01-01"
     if end is None:
         end = _1_bday_ago()
 
-    treasury = web.DataReader(
-        f"DGS{period}", data_source="fred", start=start, end=end
-    )
+    treasury = web.DataReader(f"DGS{period}", data_source="fred", start=start, end=end)
     return treasury.ffill()
 
 
 def get_symbol_returns_from_yahoo(symbol, start=None, end=None):
     """
     Wrapper for pandas.io.data.get_data_yahoo().
     Retrieves prices for symbol from yahoo and computes returns
@@ -558,7 +568,188 @@
     new_shape = (num_windows, length) + orig_shape[1:]
 
     new_strides = (array.strides[0],) + array.strides
 
     out = as_strided(array, new_shape, new_strides)
     out.setflags(write=mutable)
     return out
+
+
+def _create_unary_vectorized_roll_function(function):
+    def unary_vectorized_roll(arr, window, out=None, **kwargs):
+        """
+        Computes the {human_readable} measure over a rolling window.
+
+        Parameters
+        ----------
+        arr : array-like
+            The array to compute the rolling {human_readable} over.
+        window : int
+            Size of the rolling window in terms of the periodicity of the data.
+        out : array-like, optional
+            Array to use as output buffer.
+            If not passed, a new array will be created.
+        **kwargs
+            Forwarded to :func:`~empyrical.{name}`.
+
+        Returns
+        -------
+        rolling_{name} : array-like
+            The rolling {human_readable}.
+        """
+        allocated_output = out is None
+
+        if len(arr):
+            out = function(
+                rolling_window(_flatten(arr), min(len(arr), window)).T,
+                out=out,
+                **kwargs,
+            )
+        else:
+            out = np.empty(0, dtype="float64")
+
+        if allocated_output and isinstance(arr, pd.Series):
+            out = pd.Series(out, index=arr.index[-len(out) :])
+
+        return out
+
+    unary_vectorized_roll.__doc__ = unary_vectorized_roll.__doc__.format(
+        name=function.__name__,
+        human_readable=function.__name__.replace("_", " "),
+    )
+    unary_vectorized_roll.__name__ = f"rolling_{function.__name__}"
+
+    return unary_vectorized_roll
+
+
+def _create_binary_vectorized_roll_function(function):
+    def binary_vectorized_roll(lhs, rhs, window, out=None, **kwargs):
+        """
+        Computes the {human_readable} measure over a rolling window.
+
+        Parameters
+        ----------
+        lhs : array-like
+            The first array to pass to the rolling {human_readable}.
+        rhs : array-like
+            The second array to pass to the rolling {human_readable}.
+        window : int
+            Size of the rolling window in terms of the periodicity of the data.
+        out : array-like, optional
+            Array to use as output buffer.
+            If not passed, a new array will be created.
+        **kwargs
+            Forwarded to :func:`~empyrical.{name}`.
+
+        Returns
+        -------
+        rolling_{name} : array-like
+            The rolling {human_readable}.
+        """
+        allocated_output = out is None
+
+        if window >= 1 and len(lhs) and len(rhs):
+            out = function(
+                rolling_window(_flatten(lhs), min(len(lhs), window)).T,
+                rolling_window(_flatten(rhs), min(len(rhs), window)).T,
+                out=out,
+                **kwargs,
+            )
+        elif allocated_output:
+            out = np.empty(0, dtype="float64")
+        else:
+            out[()] = np.nan
+
+        if allocated_output:
+            if out.ndim == 1 and isinstance(lhs, pd.Series):
+                out = pd.Series(out, index=lhs.index[-len(out) :])
+            elif out.ndim == 2 and isinstance(lhs, pd.Series):
+                out = pd.DataFrame(out, index=lhs.index[-len(out) :])
+        return out
+
+    binary_vectorized_roll.__doc__ = binary_vectorized_roll.__doc__.format(
+        name=function.__name__,
+        human_readable=function.__name__.replace("_", " "),
+    )
+
+    binary_vectorized_roll.__name__ = f"rolling_{function.__name__}"
+
+    return binary_vectorized_roll
+
+
+def _flatten(arr):
+    return arr if not isinstance(arr, pd.Series) else arr.values
+
+
+def _aligned_series(*many_series):
+    """
+    Return a new list of series containing the data in the input series, but
+    with their indices aligned. NaNs will be filled in for missing values.
+
+    Parameters
+    ----------
+    *many_series
+        The series to align.
+
+    Returns
+    -------
+    aligned_series : iterable[array-like]
+        A new list of series containing the data in the input series, but
+        with their indices aligned. NaNs will be filled in for missing values.
+
+    """
+    head = many_series[0]
+    tail = many_series[1:]
+    n = len(head)
+    if isinstance(head, np.ndarray) and all(
+        len(s) == n and isinstance(s, np.ndarray) for s in tail
+    ):
+        # optimization: ndarrays of the same length are already aligned
+        return many_series
+
+    # dataframe has no ``itervalues``
+    return (v for _, v in pd.concat(map(_to_pandas, many_series), axis=1).items())
+
+
+def _to_pandas(ob):
+    """Convert an array-like to a pandas object.
+
+    Parameters
+    ----------
+    ob : array-like
+        The object to convert.
+
+    Returns
+    -------
+    pandas_structure : pd.Series or pd.DataFrame
+        The correct structure based on the dimensionality of the data.
+    """
+    if isinstance(ob, (pd.Series, pd.DataFrame)):
+        return ob
+
+    if ob.ndim == 1:
+        return pd.Series(ob)
+    elif ob.ndim == 2:
+        return pd.DataFrame(ob)
+    else:
+        raise ValueError(
+            "cannot convert array of dim > 2 to a pandas structure",
+        )
+
+
+def _adjust_returns(returns, adjustment_factor):
+    """
+    Returns the returns series adjusted by adjustment_factor. Optimizes for the
+    case of adjustment_factor being 0 by returning returns itself, not a copy!
+
+    Parameters
+    ----------
+    returns : pd.Series or np.ndarray
+    adjustment_factor : pd.Series or np.ndarray or float or int
+
+    Returns
+    -------
+    adjusted_returns : array-like
+    """
+    if isinstance(adjustment_factor, (float, int)) and adjustment_factor == 0:
+        return returns
+    return returns - adjustment_factor
```

