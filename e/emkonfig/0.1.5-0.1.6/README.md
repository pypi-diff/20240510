# Comparing `tmp/emkonfig-0.1.5.tar.gz` & `tmp/emkonfig-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emkonfig-0.1.5.tar", max compression
+gzip compressed data, was "emkonfig-0.1.6.tar", max compression
```

## Comparing `emkonfig-0.1.5.tar` & `emkonfig-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       11 2024-02-29 13:39:01.443391 emkonfig-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-03-20 15:33:07.236309 emkonfig-0.1.5/emkonfig/__init__.py
--rw-r--r--   0        0        0     1759 2024-05-10 14:02:15.140274 emkonfig-0.1.5/emkonfig/config.py
--rw-r--r--   0        0        0    18019 2024-05-10 13:51:38.329335 emkonfig-0.1.5/emkonfig/external/hydra/instantiate.py
--rw-r--r--   0        0        0     4828 2024-05-09 13:32:22.917539 emkonfig-0.1.5/emkonfig/parsers.py
--rw-r--r--   0        0        0     1052 2024-03-21 15:44:31.173249 emkonfig-0.1.5/emkonfig/registry.py
--rw-r--r--   0        0        0     1066 2024-05-10 14:22:19.135840 emkonfig-0.1.5/emkonfig/utils.py
--rw-r--r--   0        0        0     3104 2024-05-10 14:22:58.451736 emkonfig-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 emkonfig-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-02-29 13:39:01.443391 emkonfig-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 15:33:07.236309 emkonfig-0.1.6/emkonfig/__init__.py
+-rw-r--r--   0        0        0     1759 2024-05-10 14:02:15.140274 emkonfig-0.1.6/emkonfig/config.py
+-rw-r--r--   0        0        0    18019 2024-05-10 13:51:38.329335 emkonfig-0.1.6/emkonfig/external/hydra/instantiate.py
+-rw-r--r--   0        0        0     4828 2024-05-09 13:32:22.917539 emkonfig-0.1.6/emkonfig/parsers.py
+-rw-r--r--   0        0        0     1052 2024-03-21 15:44:31.173249 emkonfig-0.1.6/emkonfig/registry.py
+-rw-r--r--   0        0        0     1140 2024-05-10 14:27:16.806040 emkonfig-0.1.6/emkonfig/utils.py
+-rw-r--r--   0        0        0     3104 2024-05-10 14:27:52.832413 emkonfig-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 emkonfig-0.1.6/PKG-INFO
```

### Comparing `emkonfig-0.1.5/emkonfig/config.py` & `emkonfig-0.1.6/emkonfig/config.py`

 * *Files identical despite different names*

### Comparing `emkonfig-0.1.5/emkonfig/external/hydra/instantiate.py` & `emkonfig-0.1.6/emkonfig/external/hydra/instantiate.py`

 * *Files identical despite different names*

### Comparing `emkonfig-0.1.5/emkonfig/parsers.py` & `emkonfig-0.1.6/emkonfig/parsers.py`

 * *Files identical despite different names*

### Comparing `emkonfig-0.1.5/emkonfig/registry.py` & `emkonfig-0.1.6/emkonfig/registry.py`

 * *Files identical despite different names*

### Comparing `emkonfig-0.1.5/emkonfig/utils.py` & `emkonfig-0.1.6/emkonfig/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     exclude = set(exclude)
 
     start = time.time()
     for path in Path(dir_name).rglob("*.py"):
         if path.name.startswith("__"):
             continue
         module_path = path.with_suffix("").as_posix().replace("/", ".")
+        if verbose:
+            print(f"Importing module: {module_path}")
 
         try:
             importlib.import_module(module_path)
         except Exception as e:
             if verbose:
                 print(f"Failed to import module: {module_path}")
                 print(f"Error: {e}")
```

### Comparing `emkonfig-0.1.5/pyproject.toml` & `emkonfig-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emkonfig"
-version = "0.1.5"
+version = "0.1.6"
 description = "YAML template based configuration management tool"
 authors = ["Kıvanç Yüksel <kivanc.yuksel@emkademy.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers= [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `emkonfig-0.1.5/PKG-INFO` & `emkonfig-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emkonfig
-Version: 0.1.5
+Version: 0.1.6
 Summary: YAML template based configuration management tool
 License: MIT
 Author: Kıvanç Yüksel
 Author-email: kivanc.yuksel@emkademy.com
 Requires-Python: >=3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

