# Comparing `tmp/random_real_address-0.1.0.tar.gz` & `tmp/random_real_address-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "random_real_address-0.1.0.tar", last modified: Fri May 10 07:13:44 2024, max compression
+gzip compressed data, was "random_real_address-0.1.1.tar", last modified: Fri May 10 07:43:38 2024, max compression
```

## Comparing `random_real_address-0.1.0.tar` & `random_real_address-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:13:44.928682 random_real_address-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-10 07:13:35.000000 random_real_address-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-10 07:13:44.928682 random_real_address-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-10 07:13:35.000000 random_real_address-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-10 07:13:35.000000 random_real_address-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:13:44.924682 random_real_address-0.1.0/random_address/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:13:44.928682 random_real_address-0.1.0/random_address/random_real_address.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-10 07:13:44.000000 random_real_address-0.1.0/random_address/random_real_address.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-10 07:13:44.000000 random_real_address-0.1.0/random_address/random_real_address.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:13:44.000000 random_real_address-0.1.0/random_address/random_real_address.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-10 07:13:44.000000 random_real_address-0.1.0/random_address/random_real_address.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:13:44.000000 random_real_address-0.1.0/random_address/random_real_address.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 07:13:44.928682 random_real_address-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:13:44.928682 random_real_address-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-10 07:13:35.000000 random_real_address-0.1.0/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-10 07:13:35.000000 random_real_address-0.1.0/tests/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:43:38.561448 random_real_address-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-10 07:43:26.000000 random_real_address-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-10 07:43:38.561448 random_real_address-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-10 07:43:26.000000 random_real_address-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-10 07:43:26.000000 random_real_address-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:43:38.557448 random_real_address-0.1.1/random_address/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:43:38.561448 random_real_address-0.1.1/random_address/random_real_address.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-10 07:43:38.000000 random_real_address-0.1.1/random_address/random_real_address.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-10 07:43:38.000000 random_real_address-0.1.1/random_address/random_real_address.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:43:38.000000 random_real_address-0.1.1/random_address/random_real_address.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-10 07:43:38.000000 random_real_address-0.1.1/random_address/random_real_address.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:43:38.000000 random_real_address-0.1.1/random_address/random_real_address.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 07:43:38.561448 random_real_address-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:43:38.561448 random_real_address-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-10 07:43:26.000000 random_real_address-0.1.1/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-10 07:43:26.000000 random_real_address-0.1.1/tests/test_state.py
```

### Comparing `random_real_address-0.1.0/LICENSE` & `random_real_address-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `random_real_address-0.1.0/pyproject.toml` & `random_real_address-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "random-real-address"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python package to generate real addresses in the US."
 authors = [{name = "Naren Thiagarajan", email = "narenst@gmail.com"}]
 license = {text = "MIT License"}
 readme = "README.md"
 keywords = ["address", "random address", "US"]
 dependencies = []
```

### Comparing `random_real_address-0.1.0/tests/test_generator.py` & `random_real_address-0.1.1/tests/test_generator.py`

 * *Files identical despite different names*

