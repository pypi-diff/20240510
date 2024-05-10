# Comparing `tmp/stack_graphs_python_bindings-0.0.2.tar.gz` & `tmp/stack_graphs_python_bindings-0.0.4.tar.gz`

## Comparing `stack_graphs_python_bindings-0.0.2.tar` & `stack_graphs_python_bindings-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 stack_graphs_python_bindings-0.0.2/Cargo.toml
--rw-r--r--   0     1001      127     3486 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      730 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/.gitignore
--rw-r--r--   0     1001      127     1077 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/LICENSE
--rw-r--r--   0     1001      127      122 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/Makefile
--rw-r--r--   0     1001      127      909 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/README.md
--rw-r--r--   0     1001      127     1306 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/src/classes.rs
--rw-r--r--   0     1001      127     1870 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/src/lib.rs
--rw-r--r--   0     1001      127     3622 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/src/stack_graphs_wrapper/mod.rs
--rw-r--r--   0     1001      127      399 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/stack_graphs_python.pyi
--rw-r--r--   0     1001      127       66 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/tests/js_sample/index.js
--rw-r--r--   0     1001      127       25 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/tests/js_sample/module.js
--rw-r--r--   0     1001      127      849 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/tests/test.py
--rw-r--r--   0     1001      127    50375 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/Cargo.lock
--rw-r--r--   0     1001      127      405 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 stack_graphs_python_bindings-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 stack_graphs_python_bindings-0.0.4/Cargo.toml
+-rw-r--r--   0     1001      127     4934 2024-05-10 21:42:31.000000 stack_graphs_python_bindings-0.0.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      730 2024-05-10 21:42:31.000000 stack_graphs_python_bindings-0.0.4/.gitignore
+-rw-r--r--   0     1001      127     1077 2024-05-10 21:42:31.000000 stack_graphs_python_bindings-0.0.4/LICENSE
+-rw-r--r--   0     1001      127      122 2024-05-10 21:42:31.000000 stack_graphs_python_bindings-0.0.4/Makefile
+-rw-r--r--   0     1001      127      909 2024-05-10 21:42:31.000000 stack_graphs_python_bindings-0.0.4/README.md
+-rw-r--r--   0     1001      127     1306 2024-05-10 21:42:31.000000 stack_graphs_python_bindings-0.0.4/src/classes.rs
+-rw-r--r--   0     1001      127     1870 2024-05-10 21:42:31.000000 stack_graphs_python_bindings-0.0.4/src/lib.rs
+-rw-r--r--   0     1001      127     3622 2024-05-10 21:42:31.000000 stack_graphs_python_bindings-0.0.4/src/stack_graphs_wrapper/mod.rs
+-rw-r--r--   0     1001      127      399 2024-05-10 21:42:31.000000 stack_graphs_python_bindings-0.0.4/stack_graphs_python.pyi
+-rw-r--r--   0     1001      127       66 2024-05-10 21:42:31.000000 stack_graphs_python_bindings-0.0.4/tests/js_sample/index.js
+-rw-r--r--   0     1001      127       25 2024-05-10 21:42:31.000000 stack_graphs_python_bindings-0.0.4/tests/js_sample/module.js
+-rw-r--r--   0     1001      127      849 2024-05-10 21:42:31.000000 stack_graphs_python_bindings-0.0.4/tests/test.py
+-rw-r--r--   0     1001      127    50375 2024-05-10 21:42:31.000000 stack_graphs_python_bindings-0.0.4/Cargo.lock
+-rw-r--r--   0     1001      127      405 2024-05-10 21:42:31.000000 stack_graphs_python_bindings-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 stack_graphs_python_bindings-0.0.4/PKG-INFO
```

### Comparing `stack_graphs_python_bindings-0.0.2/Cargo.toml` & `stack_graphs_python_bindings-0.0.4/Cargo.toml`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.2/.gitignore` & `stack_graphs_python_bindings-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.2/LICENSE` & `stack_graphs_python_bindings-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.2/README.md` & `stack_graphs_python_bindings-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.2/src/classes.rs` & `stack_graphs_python_bindings-0.0.4/src/classes.rs`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.2/src/lib.rs` & `stack_graphs_python_bindings-0.0.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.2/src/stack_graphs_wrapper/mod.rs` & `stack_graphs_python_bindings-0.0.4/src/stack_graphs_wrapper/mod.rs`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.2/tests/test.py` & `stack_graphs_python_bindings-0.0.4/tests/test.py`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.2/Cargo.lock` & `stack_graphs_python_bindings-0.0.4/Cargo.lock`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.2/PKG-INFO` & `stack_graphs_python_bindings-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stack-graphs-python-bindings
-Version: 0.0.2
+Version: 0.0.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

