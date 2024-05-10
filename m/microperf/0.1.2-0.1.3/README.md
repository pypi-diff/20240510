# Comparing `tmp/microperf-0.1.2.tar.gz` & `tmp/microperf-0.1.3.tar.gz`

## Comparing `microperf-0.1.2.tar` & `microperf-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 microperf-0.1.2/build-perf.py
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 microperf-0.1.2/patterns.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 microperf-0.1.2/perf-script.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 microperf-0.1.2/ratio.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 microperf-0.1.2/.github/workflows/release.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 microperf-0.1.2/presto/Dockerfile
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 microperf-0.1.2/presto/etc/config.properties
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 microperf-0.1.2/presto/etc/jvm.config
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 microperf-0.1.2/presto/etc/node.properties
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 microperf-0.1.2/presto/etc/catalog/memory.properties
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 microperf-0.1.2/src/microperf/__init__.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 microperf-0.1.2/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 microperf-0.1.2/LICENSE
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 microperf-0.1.2/README.md
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 microperf-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 microperf-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 microperf-0.1.3/Cargo.toml
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 microperf-0.1.3/build-perf.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 microperf-0.1.3/check-version-bump.py
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 microperf-0.1.3/patterns.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 microperf-0.1.3/perf-script.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 microperf-0.1.3/ratio.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 microperf-0.1.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 microperf-0.1.3/presto/Dockerfile
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 microperf-0.1.3/presto/etc/config.properties
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 microperf-0.1.3/presto/etc/jvm.config
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 microperf-0.1.3/presto/etc/node.properties
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 microperf-0.1.3/presto/etc/catalog/memory.properties
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 microperf-0.1.3/src/lib.rs
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 microperf-0.1.3/src/microperf/__init__.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 microperf-0.1.3/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 microperf-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 microperf-0.1.3/README.md
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 microperf-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 microperf-0.1.3/PKG-INFO
```

### Comparing `microperf-0.1.2/build-perf.py` & `microperf-0.1.3/build-perf.py`

 * *Files identical despite different names*

### Comparing `microperf-0.1.2/patterns.py` & `microperf-0.1.3/patterns.py`

 * *Files identical despite different names*

### Comparing `microperf-0.1.2/perf-script.py` & `microperf-0.1.3/perf-script.py`

 * *Files identical despite different names*

### Comparing `microperf-0.1.2/ratio.py` & `microperf-0.1.3/ratio.py`

 * *Files identical despite different names*

### Comparing `microperf-0.1.2/.github/workflows/release.yml` & `microperf-0.1.3/.github/workflows/release.yml`

 * *Files 14% similar despite different names*

```diff
@@ -9,24 +9,32 @@
   id-token: write
 
 jobs:
   release:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v4
+      - uses: actions/checkout@v4
 
-    - name: Set up Python
-      uses: actions/setup-python@v4
-      with:
-        python-version: '3.x'
-
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install build
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: "3.x"
+
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install build packaging requests
+
+      - name: Check version bump
+        run: python3 check-version-bump.py
+
+      - name: Build package
+        run: python -m build
+
+      - name: Publish to crates.io
+        run: |
+          cargo login ${{ secrets.CRATES_IO_API_TOKEN }}
+          cargo publish --allow-dirty
 
-    - name: Build package
-      run: python -m build
-
-    - name: Publish package
-      uses: pypa/gh-action-pypi-publish@release/v1
+      - name: Publish to PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `microperf-0.1.2/presto/Dockerfile` & `microperf-0.1.3/presto/Dockerfile`

 * *Files identical despite different names*

### Comparing `microperf-0.1.2/LICENSE` & `microperf-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `microperf-0.1.2/README.md` & `microperf-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `microperf-0.1.2/pyproject.toml` & `microperf-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "microperf"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Nicolas van Kempen", email="nvankemp@gmail.com" },
 ]
 dependencies = ["presto-python-client==0.8.4"]
 description = "A small tool using perf to provide more performance insights."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `microperf-0.1.2/PKG-INFO` & `microperf-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: microperf
-Version: 0.1.2
+Version: 0.1.3
 Summary: A small tool using perf to provide more performance insights.
 Project-URL: Homepage, https://github.com/nicovank/microperf
 Project-URL: Bug Tracker, https://github.com/nicovank/microperf/issues
 Author-email: Nicolas van Kempen <nvankemp@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

