# Comparing `tmp/zenflow-0.1.2.tar.gz` & `tmp/zenflow-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenflow-0.1.2.tar", last modified: Fri May 10 15:26:14 2024, max compression
+gzip compressed data, was "zenflow-0.1.4.tar", last modified: Fri May 10 15:46:14 2024, max compression
```

## Comparing `zenflow-0.1.2.tar` & `zenflow-0.1.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2024-05-10 15:26:14.043078 zenflow-0.1.2/
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2024-05-10 15:26:14.016318 zenflow-0.1.2/.github/
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2024-05-10 15:26:14.019360 zenflow-0.1.2/.github/workflows/
--rw-r--r--   0 hdembinski   (501) staff       (20)      860 2024-05-10 15:25:35.000000 zenflow-0.1.2/.github/workflows/release.yml
--rw-r--r--   0 hdembinski   (501) staff       (20)      861 2024-05-10 15:09:38.000000 zenflow-0.1.2/.github/workflows/test.yml
--rw-r--r--   0 hdembinski   (501) staff       (20)       49 2024-04-05 10:36:05.000000 zenflow-0.1.2/.gitignore
--rw-r--r--   0 hdembinski   (501) staff       (20)     1557 2024-02-28 10:12:57.000000 zenflow-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 hdembinski   (501) staff       (20)     1095 2024-02-27 10:13:23.000000 zenflow-0.1.2/LICENSE
--rw-r--r--   0 hdembinski   (501) staff       (20)     1299 2024-05-10 15:26:14.042341 zenflow-0.1.2/PKG-INFO
--rw-r--r--   0 hdembinski   (501) staff       (20)      541 2024-05-10 14:29:15.000000 zenflow-0.1.2/README.md
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2024-05-10 15:26:14.029847 zenflow-0.1.2/examples/
--rw-r--r--   0 hdembinski   (501) staff       (20)   174652 2024-05-10 15:25:35.000000 zenflow-0.1.2/examples/bijectors.ipynb
--rw-r--r--   0 hdembinski   (501) staff       (20)   505994 2024-05-10 15:25:35.000000 zenflow-0.1.2/examples/deep_set.ipynb
--rw-r--r--   0 hdembinski   (501) staff       (20)  1665737 2024-05-10 15:25:35.000000 zenflow-0.1.2/examples/distributions.ipynb
--rw-r--r--   0 hdembinski   (501) staff       (20)    67089 2024-05-10 15:25:35.000000 zenflow-0.1.2/examples/one_dimensional_distribution.ipynb
--rw-r--r--   0 hdembinski   (501) staff       (20)   947901 2024-05-10 15:25:35.000000 zenflow-0.1.2/examples/two_moons.ipynb
--rw-r--r--   0 hdembinski   (501) staff       (20)   806669 2024-05-10 15:25:35.000000 zenflow-0.1.2/examples/two_moons_conditional.ipynb
--rw-r--r--   0 hdembinski   (501) staff       (20)     1403 2024-05-10 15:25:35.000000 zenflow-0.1.2/pyproject.toml
--rw-r--r--   0 hdembinski   (501) staff       (20)       38 2024-05-10 15:26:14.043227 zenflow-0.1.2/setup.cfg
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2024-05-10 15:26:14.016849 zenflow-0.1.2/src/
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2024-05-10 15:26:14.034948 zenflow-0.1.2/src/zenflow/
--rw-r--r--   0 hdembinski   (501) staff       (20)      114 2024-05-10 15:25:35.000000 zenflow-0.1.2/src/zenflow/__init__.py
--rw-r--r--   0 hdembinski   (501) staff       (20)    10829 2024-05-10 15:25:35.000000 zenflow-0.1.2/src/zenflow/bijectors.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     3692 2024-05-10 15:25:35.000000 zenflow-0.1.2/src/zenflow/distributions.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     3355 2024-05-10 15:25:35.000000 zenflow-0.1.2/src/zenflow/flow.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      430 2024-05-10 15:25:35.000000 zenflow-0.1.2/src/zenflow/layer_utils.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     4204 2024-05-10 15:25:35.000000 zenflow-0.1.2/src/zenflow/train.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     7659 2024-05-10 15:25:35.000000 zenflow-0.1.2/src/zenflow/utils.py
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2024-05-10 15:26:14.040202 zenflow-0.1.2/src/zenflow.egg-info/
--rw-r--r--   0 hdembinski   (501) staff       (20)     1299 2024-05-10 15:26:13.000000 zenflow-0.1.2/src/zenflow.egg-info/PKG-INFO
--rw-r--r--   0 hdembinski   (501) staff       (20)      760 2024-05-10 15:26:14.000000 zenflow-0.1.2/src/zenflow.egg-info/SOURCES.txt
--rw-r--r--   0 hdembinski   (501) staff       (20)        1 2024-05-10 15:26:13.000000 zenflow-0.1.2/src/zenflow.egg-info/dependency_links.txt
--rw-r--r--   0 hdembinski   (501) staff       (20)      117 2024-05-10 15:26:13.000000 zenflow-0.1.2/src/zenflow.egg-info/requires.txt
--rw-r--r--   0 hdembinski   (501) staff       (20)        8 2024-05-10 15:26:13.000000 zenflow-0.1.2/src/zenflow.egg-info/top_level.txt
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2024-05-10 15:26:14.039608 zenflow-0.1.2/tests/
--rw-r--r--   0 hdembinski   (501) staff       (20)     3901 2024-05-10 15:25:35.000000 zenflow-0.1.2/tests/test_bijectors.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1897 2024-05-10 15:25:35.000000 zenflow-0.1.2/tests/test_distributions.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      938 2024-05-10 15:25:35.000000 zenflow-0.1.2/tests/test_flow.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      476 2024-05-10 15:25:35.000000 zenflow-0.1.2/tests/test_train.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     2787 2024-05-10 15:25:35.000000 zenflow-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:46:14.755095 zenflow-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:46:14.743095 zenflow-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:46:14.743095 zenflow-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-10 15:46:04.000000 zenflow-0.1.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 15:46:04.000000 zenflow-0.1.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 15:46:04.000000 zenflow-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-10 15:46:04.000000 zenflow-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-10 15:46:04.000000 zenflow-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-10 15:46:14.755095 zenflow-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-10 15:46:04.000000 zenflow-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:46:14.751095 zenflow-0.1.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   174652 2024-05-10 15:46:04.000000 zenflow-0.1.4/examples/bijectors.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   505994 2024-05-10 15:46:04.000000 zenflow-0.1.4/examples/deep_set.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1665737 2024-05-10 15:46:04.000000 zenflow-0.1.4/examples/distributions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    67089 2024-05-10 15:46:04.000000 zenflow-0.1.4/examples/one_dimensional_distribution.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   947901 2024-05-10 15:46:04.000000 zenflow-0.1.4/examples/two_moons.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   806669 2024-05-10 15:46:04.000000 zenflow-0.1.4/examples/two_moons_conditional.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-10 15:46:04.000000 zenflow-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:46:14.755095 zenflow-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:46:14.743095 zenflow-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:46:14.751095 zenflow-0.1.4/src/zenflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-10 15:46:04.000000 zenflow-0.1.4/src/zenflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-10 15:46:04.000000 zenflow-0.1.4/src/zenflow/bijectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-10 15:46:04.000000 zenflow-0.1.4/src/zenflow/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-10 15:46:04.000000 zenflow-0.1.4/src/zenflow/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-10 15:46:04.000000 zenflow-0.1.4/src/zenflow/layer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-10 15:46:04.000000 zenflow-0.1.4/src/zenflow/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-05-10 15:46:04.000000 zenflow-0.1.4/src/zenflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:46:14.755095 zenflow-0.1.4/src/zenflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-10 15:46:14.000000 zenflow-0.1.4/src/zenflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-10 15:46:14.000000 zenflow-0.1.4/src/zenflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:46:14.000000 zenflow-0.1.4/src/zenflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-10 15:46:14.000000 zenflow-0.1.4/src/zenflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 15:46:14.000000 zenflow-0.1.4/src/zenflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:46:14.755095 zenflow-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-10 15:46:04.000000 zenflow-0.1.4/tests/test_bijectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-10 15:46:04.000000 zenflow-0.1.4/tests/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-10 15:46:04.000000 zenflow-0.1.4/tests/test_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-10 15:46:04.000000 zenflow-0.1.4/tests/test_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-10 15:46:04.000000 zenflow-0.1.4/tests/test_utils.py
```

### Comparing `zenflow-0.1.2/.github/workflows/release.yml` & `zenflow-0.1.4/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -29,12 +29,12 @@
           fetch-depth: 0  # needed by setuptools_scm
     - uses: actions/setup-python@v5
       with:
         python-version: '3.11'
 
     - run: python -m pip install --upgrade pip build
     - run: python -m build
-    - run: python -m pip install --prefer-binary $(echo dist/*.whl)'[test]'
-    - run: python -m pytest
+    # - run: python -m pip install --prefer-binary $(echo dist/*.whl)'[test]'
+    # - run: python -m pytest
 
     - uses: pypa/gh-action-pypi-publish@release/v1
       if: github.event_name == 'push' && contains(github.event.ref, '/tags/')
```

### Comparing `zenflow-0.1.2/.github/workflows/test.yml` & `zenflow-0.1.4/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         include:
           # version number must be string, otherwise 3.10 becomes 3.1
           - os: windows-latest
             python-version: "3.12"
           - os: ubuntu-latest
             python-version: "3.10"
           - os: macos-latest
-            python-version: "3.8"
+            python-version: "3.9"
       fail-fast: false
 
     runs-on: ${{ matrix.os }}
 
     steps:
     - uses: actions/checkout@v4
     - uses: actions/setup-python@v5
```

### Comparing `zenflow-0.1.2/.pre-commit-config.yaml` & `zenflow-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/LICENSE` & `zenflow-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/PKG-INFO` & `zenflow-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: zenflow
-Version: 0.1.2
+Version: 0.1.4
 Summary: Learn distributions with normalizing flows.
 Author: Hans Dembinski
 Author-email: hans.dembinski@gmail.com
-Project-URL: repository, https://github.com/hdembinski/neural_flow
+Project-URL: repository, https://github.com/hdembinski/zenflow
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: flax
 Requires-Dist: optax
```

### Comparing `zenflow-0.1.2/README.md` & `zenflow-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/examples/bijectors.ipynb` & `zenflow-0.1.4/examples/bijectors.ipynb`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/examples/deep_set.ipynb` & `zenflow-0.1.4/examples/deep_set.ipynb`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/examples/distributions.ipynb` & `zenflow-0.1.4/examples/distributions.ipynb`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/examples/one_dimensional_distribution.ipynb` & `zenflow-0.1.4/examples/one_dimensional_distribution.ipynb`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/examples/two_moons.ipynb` & `zenflow-0.1.4/examples/two_moons.ipynb`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/examples/two_moons_conditional.ipynb` & `zenflow-0.1.4/examples/two_moons_conditional.ipynb`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/pyproject.toml` & `zenflow-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 authors = [{ name = "Hans Dembinski" }, { email = "hans.dembinski@gmail.com" }]
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["jax", "jaxlib", "flax", "optax", "jaxtyping"]
 dynamic = ["version"]
 
 [project.urls]
-repository = "https://github.com/hdembinski/neural_flow"
+repository = "https://github.com/hdembinski/zenflow"
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov", "coverage[toml]", "jacobi"]
 all = ["matplotlib", "scikit-learn", "numpy"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `zenflow-0.1.2/src/zenflow/bijectors.py` & `zenflow-0.1.4/src/zenflow/bijectors.py`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/src/zenflow/distributions.py` & `zenflow-0.1.4/src/zenflow/distributions.py`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/src/zenflow/flow.py` & `zenflow-0.1.4/src/zenflow/flow.py`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/src/zenflow/train.py` & `zenflow-0.1.4/src/zenflow/train.py`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/src/zenflow/utils.py` & `zenflow-0.1.4/src/zenflow/utils.py`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/src/zenflow.egg-info/PKG-INFO` & `zenflow-0.1.4/src/zenflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: zenflow
-Version: 0.1.2
+Version: 0.1.4
 Summary: Learn distributions with normalizing flows.
 Author: Hans Dembinski
 Author-email: hans.dembinski@gmail.com
-Project-URL: repository, https://github.com/hdembinski/neural_flow
+Project-URL: repository, https://github.com/hdembinski/zenflow
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: flax
 Requires-Dist: optax
```

### Comparing `zenflow-0.1.2/src/zenflow.egg-info/SOURCES.txt` & `zenflow-0.1.4/src/zenflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/tests/test_bijectors.py` & `zenflow-0.1.4/tests/test_bijectors.py`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/tests/test_distributions.py` & `zenflow-0.1.4/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/tests/test_flow.py` & `zenflow-0.1.4/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `zenflow-0.1.2/tests/test_utils.py` & `zenflow-0.1.4/tests/test_utils.py`

 * *Files identical despite different names*

