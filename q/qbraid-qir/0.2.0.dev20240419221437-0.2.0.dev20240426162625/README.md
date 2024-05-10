# Comparing `tmp/qbraid_qir-0.2.0.dev20240419221437.tar.gz` & `tmp/qbraid_qir-0.2.0.dev20240426162625.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid_qir-0.2.0.dev20240419221437.tar", last modified: Fri Apr 19 22:14:39 2024, max compression
+gzip compressed data, was "qbraid_qir-0.2.0.dev20240426162625.tar", last modified: Fri Apr 26 16:26:28 2024, max compression
```

## Comparing `qbraid_qir-0.2.0.dev20240419221437.tar` & `qbraid_qir-0.2.0.dev20240426162625.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.912293 qbraid_qir-0.2.0.dev20240419221437/
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    49311 2024-04-19 22:14:39.912293 qbraid_qir-0.2.0.dev20240419221437/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.904293 qbraid_qir-0.2.0.dev20240419221437/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.904293 qbraid_qir-0.2.0.dev20240419221437/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.904293 qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/
--rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/cirq.png
--rw-r--r--   0 runner    (1001) docker     (127)    32358 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/qbraid.png
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/qir.png
--rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/qosf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.904293 qbraid_qir-0.2.0.dev20240419221437/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/api/qbraid_qir.cirq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/api/qbraid_qir.qasm3.rst
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/api/qbraid_qir.rst
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/api/qbraid_qir.runner.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.904293 qbraid_qir-0.2.0.dev20240419221437/docs/userguide/
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/userguide/cirq_qir.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/userguide/qasm3_qir.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/docs/userguide/qasm3_supported.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.904293 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 22:14:37.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.908293 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/opsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/passes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.908293 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/oq3_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)    34547 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.908293 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.908293 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    49311 2024-04-19 22:14:39.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-19 22:14:39.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 22:14:39.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-19 22:14:39.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 22:14:39.000000 qbraid_qir-0.2.0.dev20240419221437/qbraid_qir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 22:14:39.912293 qbraid_qir-0.2.0.dev20240419221437/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:14:39.908293 qbraid_qir-0.2.0.dev20240419221437/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5254 2024-04-19 22:14:34.000000 qbraid_qir-0.2.0.dev20240419221437/tools/verify_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:26:28.549049 qbraid_qir-0.2.0.dev20240426162625/
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    49175 2024-04-26 16:26:28.549049 qbraid_qir-0.2.0.dev20240426162625/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:26:28.537048 qbraid_qir-0.2.0.dev20240426162625/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:26:28.541048 qbraid_qir-0.2.0.dev20240426162625/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:26:28.541048 qbraid_qir-0.2.0.dev20240426162625/docs/_static/pkg-logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/docs/_static/pkg-logos/cirq.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32358 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/docs/_static/pkg-logos/qbraid.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/docs/_static/pkg-logos/qir.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/docs/_static/pkg-logos/qosf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:26:28.541048 qbraid_qir-0.2.0.dev20240426162625/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/docs/api/qbraid_qir.cirq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/docs/api/qbraid_qir.qasm3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/docs/api/qbraid_qir.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/docs/api/qbraid_qir.runner.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:26:28.541048 qbraid_qir-0.2.0.dev20240426162625/docs/userguide/
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/docs/userguide/cirq_qir.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/docs/userguide/qasm3_qir.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/docs/userguide/qasm3_supported.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:26:28.541048 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-26 16:26:25.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:26:28.545048 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/cirq/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/cirq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/cirq/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/cirq/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/cirq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/cirq/opsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/cirq/passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/cirq/visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:26:28.545048 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/qasm3/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/qasm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/qasm3/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/qasm3/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/qasm3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/qasm3/oq3_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47928 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/qasm3/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:26:28.545048 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/runner/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/runner/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/runner/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:26:28.545048 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49175 2024-04-26 16:26:28.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-26 16:26:28.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:26:28.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-26 16:26:28.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 16:26:28.000000 qbraid_qir-0.2.0.dev20240426162625/qbraid_qir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:26:28.549049 qbraid_qir-0.2.0.dev20240426162625/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:26:28.545048 qbraid_qir-0.2.0.dev20240426162625/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5254 2024-04-26 16:26:19.000000 qbraid_qir-0.2.0.dev20240426162625/tools/verify_headers.py
```

### Comparing `qbraid_qir-0.2.0.dev20240419221437/CODE_OF_CONDUCT.md` & `qbraid_qir-0.2.0.dev20240426162625/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/CONTRIBUTING.md` & `qbraid_qir-0.2.0.dev20240426162625/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/LICENSE` & `qbraid_qir-0.2.0.dev20240426162625/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/PKG-INFO` & `qbraid_qir-0.2.0.dev20240426162625/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-qir
-Version: 0.2.0.dev20240419221437
+Version: 0.2.0.dev20240426162625
 Summary: qBraid-SDK extension providing support for QIR conversions.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -710,16 +710,16 @@
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: lint
 Requires-Dist: black[jupyter]; extra == "lint"
 Requires-Dist: isort; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Provides-Extra: docs
-Requires-Dist: sphinx~=7.2.6; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints<2.1,>=1.24; extra == "docs"
+Requires-Dist: sphinx~=7.3.7; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints<2.2,>=1.24; extra == "docs"
 Requires-Dist: sphinx-rtd-theme~=2.0.0; extra == "docs"
 Requires-Dist: docutils<0.22; extra == "docs"
 
 <img width="full" alt="qbraid-qir-header" src="https://github.com/qBraid/qbraid-qir/assets/46977852/39f921ae-c4bf-442a-b059-6b21abd2ae50">
 
 <p align='center'>
   <a href='https://github.com/qBraid/qbraid-qir/actions/workflows/main.yml'>
@@ -857,16 +857,14 @@
 """
 
 module = qasm3_to_qir(program, name="my-program")
 
 ir = str(module)
 ```
 
-[Currently Supported Operations](https://docs.google.com/spreadsheets/d/1Jgo2_usAnCmV5OLK1RvaGzd7vdjKZKxoBvlTI3g1_lE/edit?usp=sharing)
-
 ### Add QIR node to qBraid conversion graph
 
 ```python
 from qbraid_qir.cirq import cirq_to_qir
 from qbraid.transpiler import Conversion, ConversionGraph
 
 graph = ConversionGraph()
```

### Comparing `qbraid_qir-0.2.0.dev20240419221437/README.md` & `qbraid_qir-0.2.0.dev20240426162625/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -136,16 +136,14 @@
 """
 
 module = qasm3_to_qir(program, name="my-program")
 
 ir = str(module)
 ```
 
-[Currently Supported Operations](https://docs.google.com/spreadsheets/d/1Jgo2_usAnCmV5OLK1RvaGzd7vdjKZKxoBvlTI3g1_lE/edit?usp=sharing)
-
 ### Add QIR node to qBraid conversion graph
 
 ```python
 from qbraid_qir.cirq import cirq_to_qir
 from qbraid.transpiler import Conversion, ConversionGraph
 
 graph = ConversionGraph()
```

#### html2text {}

```diff
@@ -30,33 +30,32 @@
 examples ### Cirq conversions ```python import cirq from qbraid_qir.cirq import
 cirq_to_qir q0, q1 = cirq.LineQubit.range(2) circuit = cirq.Circuit( cirq.H
 (q0), cirq.CNOT(q0, q1), cirq.measure(q0, q1) ) module = cirq_to_qir(circuit,
 name="my-circuit") ir = str(module) ``` ### OpenQASM 3 conversions ```python
 from qbraid_qir.qasm3 import qasm3_to_qir program = """ OPENQASM 3; include
 "stdgates.inc"; qubit[2] q; bit[2] c; h q[0]; cx q[0], q[1]; measure q[0] -> c
 [0]; measure q[1] -> c[1]; """ module = qasm3_to_qir(program, name="my-
-program") ir = str(module) ``` [Currently Supported Operations](https://
-docs.google.com/spreadsheets/d/1Jgo2_usAnCmV5OLK1RvaGzd7vdjKZKxoBvlTI3g1_lE/
-edit?usp=sharing) ### Add QIR node to qBraid conversion graph ```python from
-qbraid_qir.cirq import cirq_to_qir from qbraid.transpiler import Conversion,
-ConversionGraph graph = ConversionGraph() conversion = Conversion("cirq",
-"qir", cirq_to_qir) graph.add_conversion(conversion) graph.plot() ``` ##
-Architecture diagram qBraid-SDK transpiler hub-and-spokes [architecture](https:
-//docs.qbraid.com/en/latest/sdk/transpiler.html#architecture) with qbraid-qir
-integration (left) mapped to language specific conversion step in QIR
-abstraction [layers](https://www.qir-alliance.org/qir-book/concepts/why-do-we-
-need.html) (right). [architecture]## Contributing - Interested in contributing
-code, or making a PR? See [CONTRIBUTING.md](CONTRIBUTING.md) - For feature
-requests and bug reports: [Submit an issue](https://github.com/qBraid/qbraid-
-qir/issues) - For discussions, and specific questions about the qBraid-SDK,
-qBraid-QIR, or other topics, [join our discord community](https://discord.gg/
-TPBU2sa8Et) - For questions that are more suited for a forum, post to [Quantum
-Computing Stack Exchange](https://quantumcomputing.stackexchange.com/) with the
-[`qbraid`](https://quantumcomputing.stackexchange.com/questions/tagged/qbraid)
-tag. - By participating, you are expected to uphold our [code of conduct]
+program") ir = str(module) ``` ### Add QIR node to qBraid conversion graph
+```python from qbraid_qir.cirq import cirq_to_qir from qbraid.transpiler import
+Conversion, ConversionGraph graph = ConversionGraph() conversion = Conversion
+("cirq", "qir", cirq_to_qir) graph.add_conversion(conversion) graph.plot() ```
+## Architecture diagram qBraid-SDK transpiler hub-and-spokes [architecture]
+(https://docs.qbraid.com/en/latest/sdk/transpiler.html#architecture) with
+qbraid-qir integration (left) mapped to language specific conversion step in
+QIR abstraction [layers](https://www.qir-alliance.org/qir-book/concepts/why-do-
+we-need.html) (right). [architecture]## Contributing - Interested in
+contributing code, or making a PR? See [CONTRIBUTING.md](CONTRIBUTING.md) - For
+feature requests and bug reports: [Submit an issue](https://github.com/qBraid/
+qbraid-qir/issues) - For discussions, and specific questions about the qBraid-
+SDK, qBraid-QIR, or other topics, [join our discord community](https://
+discord.gg/TPBU2sa8Et) - For questions that are more suited for a forum, post
+to [Quantum Computing Stack Exchange](https://
+quantumcomputing.stackexchange.com/) with the [`qbraid`](https://
+quantumcomputing.stackexchange.com/questions/tagged/qbraid) tag. - By
+participating, you are expected to uphold our [code of conduct]
 (CODE_OF_CONDUCT). ## Citation If you use qBraid-QIR in your research, we
 kindly request that you cite it appropriately. The BibTeX entry below is
 aligned with the latest stable release. For the most up-to-date citation
 details, please refer to [CITATION.cff](CITATION.cff). ```tex @software
 {Kushnir_qBraid-QIR_Python_package_2024, author = {Kushnir, Samuel and Gupta,
 Harshit and Jain, Rohan and Parakh, Priyansh and Hill, Ryan James}, license =
 {GPL-3.0}, month = mar, title = {{qBraid-QIR: Python package for QIR
```

### Comparing `qbraid_qir-0.2.0.dev20240419221437/docs/_static/favicon.ico` & `qbraid_qir-0.2.0.dev20240426162625/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/docs/_static/logo.png` & `qbraid_qir-0.2.0.dev20240426162625/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/cirq.png` & `qbraid_qir-0.2.0.dev20240426162625/docs/_static/pkg-logos/cirq.png`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/qbraid.png` & `qbraid_qir-0.2.0.dev20240426162625/docs/_static/pkg-logos/qbraid.png`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/qir.png` & `qbraid_qir-0.2.0.dev20240426162625/docs/_static/pkg-logos/qir.png`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/docs/_static/pkg-logos/qosf.png` & `qbraid_qir-0.2.0.dev20240426162625/docs/_static/pkg-logos/qosf.png`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/docs/conf.py` & `qbraid_qir-0.2.0.dev20240426162625/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/docs/index.rst` & `qbraid_qir-0.2.0.dev20240426162625/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/docs/userguide/cirq_qir.rst` & `qbraid_qir-0.2.0.dev20240426162625/docs/userguide/cirq_qir.rst`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/docs/userguide/qasm3_qir.rst` & `qbraid_qir-0.2.0.dev20240426162625/docs/userguide/qasm3_qir.rst`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/docs/userguide/qasm3_supported.rst` & `qbraid_qir-0.2.0.dev20240426162625/docs/userguide/qasm3_supported.rst`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/pyproject.toml` & `qbraid_qir-0.2.0.dev20240426162625/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 "Launch on Lab" = "https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qbraid-qir.git"
 
 [project.optional-dependencies]
 cirq = ["cirq-core>=1.3.0,<1.4.0"]
 qasm3 = ["openqasm3[parser]>=0.4.0,<0.6.0"]
 test = ["qbraid>=0.5.3,<0.7.0", "pytest", "pytest-cov"]
 lint = ["black[jupyter]", "isort", "pylint"]
-docs = ["sphinx~=7.2.6", "sphinx-autodoc-typehints>=1.24,<2.1", "sphinx-rtd-theme~=2.0.0", "docutils<0.22"]
+docs = ["sphinx~=7.3.7", "sphinx-autodoc-typehints>=1.24,<2.2", "sphinx-rtd-theme~=2.0.0", "docutils<0.22"]
 
 [tool.setuptools.dynamic]
 version = {attr = "qbraid_qir.__version__"}
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length = 100
 disable = "C0103, C0115, C0116, I1101, R0903, W0212, W0511"
```

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/__init__.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/__init__.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/cirq/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/convert.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/cirq/convert.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/elements.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/cirq/elements.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/exceptions.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/cirq/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/opsets.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/cirq/opsets.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/passes.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/cirq/passes.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/cirq/visitor.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/cirq/visitor.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/exceptions.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/__init__.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/qasm3/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/convert.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/qasm3/convert.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/elements.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/qasm3/elements.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,41 +29,54 @@
 
     """
     # TODO: Consider a better approach of generating a unique identifier.
     generated_id = uuid.uuid1()
     return f"program-{generated_id}"
 
 
-class Scope(Enum):
-    """
-    Enum for the different scopes in QIR.
-
-    """
-
-    GLOBAL = "global"
-    GATE = "gate"
-    FUNCTION = "function"
-
-
 class Context(Enum):
     """
     Enum for the different contexts in QIR.
 
     """
 
     GLOBAL = "global"
     IF = "if"
     LOOP = "loop"
+    FUNCTION = "function"
 
 
 class InversionOp(Enum):
     NO_OP = 1
     INVERT_ROTATION = 2
 
 
+class Variable:
+    """
+    Class representing an openqasm variable.
+
+    Args:
+        name (str): Name of the variable.
+        base_type (Any): Base type of the variable.
+        base_size (int): Base size of the variable.
+        dims (List[int]): Dimensions of the variable.
+        value (Optional[Union[int, float, list]]): Value of the variable.
+        is_constant (bool): Flag indicating if the variable is constant.
+
+    """
+
+    def __init__(self, name, base_type, base_size, dims, value, is_constant=False):
+        self.name = name
+        self.base_type = base_type
+        self.base_size = base_size
+        self.dims = dims
+        self.value = value
+        self.is_constant = is_constant
+
+
 class _ProgramElement(metaclass=ABCMeta):
     @classmethod
     def from_element_list(cls, elements):
         return [cls(elem) for elem in elements]
 
     @abstractmethod
     def accept(self, visitor):
@@ -150,14 +163,18 @@
 
             elif isinstance(statement, ClassicalDeclaration) and isinstance(
                 statement.type, BitType
             ):
                 size = 1 if statement.type.size is None else statement.type.size.value
                 num_clbits += size
                 elements.append(_Register(statement))
+                # as bit arrays are just 0 / 1 values, we can treat them as
+                # classical variables too. Thus, need to add them to normal
+                # statements too.
+                elements.append(_Statement(statement))
             else:
                 elements.append(_Statement(statement))
 
         if module is None:
             # pylint: disable-next=too-many-function-args
             module = Module(qirContext(), generate_module_id(program))
```

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/exceptions.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/qasm3/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/qasm3/oq3_maps.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/qasm3/oq3_maps.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,24 @@
 Module mapping supported QASM gates/operations to pyqir functions.
 
 """
 
 from typing import Union
 
 import pyqir
+from openqasm3.ast import (
+    AngleType,
+    ArrayType,
+    BitType,
+    BoolType,
+    ComplexType,
+    FloatType,
+    IntType,
+    UintType,
+)
 
 from .elements import InversionOp
 from .exceptions import Qasm3ConversionError
 
 OPERATOR_MAP = {
     "+": lambda x, y: x + y,
     "-": lambda x, y: x - y,
@@ -240,10 +250,17 @@
 CONSTANTS_MAP = {
     "pi": 3.141592653589793,
     "π": 3.141592653589793,
     "e": 2.718281828459045,
     "tau": 6.283185307179586,
 }
 
-
-def qasm3_constants_map(constant_name: str):
-    return CONSTANTS_MAP[constant_name]
+VARIABLE_TYPE_MAP = {
+    BitType: bool,
+    IntType: int,
+    UintType: int,
+    BoolType: bool,
+    FloatType: float,
+    ArrayType: None,  # not sure
+    AngleType: None,  # not sure
+    ComplexType: complex,
+}
```

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/__init__.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/exceptions.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/runner/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/result.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/runner/result.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/runner/simulator.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/runner/simulator.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir/serialization.py` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir/serialization.py`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir.egg-info/PKG-INFO` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-qir
-Version: 0.2.0.dev20240419221437
+Version: 0.2.0.dev20240426162625
 Summary: qBraid-SDK extension providing support for QIR conversions.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -710,16 +710,16 @@
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: lint
 Requires-Dist: black[jupyter]; extra == "lint"
 Requires-Dist: isort; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Provides-Extra: docs
-Requires-Dist: sphinx~=7.2.6; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints<2.1,>=1.24; extra == "docs"
+Requires-Dist: sphinx~=7.3.7; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints<2.2,>=1.24; extra == "docs"
 Requires-Dist: sphinx-rtd-theme~=2.0.0; extra == "docs"
 Requires-Dist: docutils<0.22; extra == "docs"
 
 <img width="full" alt="qbraid-qir-header" src="https://github.com/qBraid/qbraid-qir/assets/46977852/39f921ae-c4bf-442a-b059-6b21abd2ae50">
 
 <p align='center'>
   <a href='https://github.com/qBraid/qbraid-qir/actions/workflows/main.yml'>
@@ -857,16 +857,14 @@
 """
 
 module = qasm3_to_qir(program, name="my-program")
 
 ir = str(module)
 ```
 
-[Currently Supported Operations](https://docs.google.com/spreadsheets/d/1Jgo2_usAnCmV5OLK1RvaGzd7vdjKZKxoBvlTI3g1_lE/edit?usp=sharing)
-
 ### Add QIR node to qBraid conversion graph
 
 ```python
 from qbraid_qir.cirq import cirq_to_qir
 from qbraid.transpiler import Conversion, ConversionGraph
 
 graph = ConversionGraph()
```

### Comparing `qbraid_qir-0.2.0.dev20240419221437/qbraid_qir.egg-info/SOURCES.txt` & `qbraid_qir-0.2.0.dev20240426162625/qbraid_qir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qbraid_qir-0.2.0.dev20240419221437/tools/verify_headers.py` & `qbraid_qir-0.2.0.dev20240426162625/tools/verify_headers.py`

 * *Files identical despite different names*

