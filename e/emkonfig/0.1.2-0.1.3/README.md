# Comparing `tmp/emkonfig-0.1.2.tar.gz` & `tmp/emkonfig-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emkonfig-0.1.2.tar", max compression
+gzip compressed data, was "emkonfig-0.1.3.tar", max compression
```

## Comparing `emkonfig-0.1.2.tar` & `emkonfig-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0       11 2024-02-29 13:39:01.443391 emkonfig-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-03-20 15:33:07.236309 emkonfig-0.1.2/emkonfig/__init__.py
--rw-r--r--   0        0        0     1589 2024-04-23 12:32:00.439509 emkonfig-0.1.2/emkonfig/config.py
--rw-r--r--   0        0        0     4828 2024-05-09 13:32:22.917539 emkonfig-0.1.2/emkonfig/parsers.py
--rw-r--r--   0        0        0     1052 2024-03-21 15:44:31.173249 emkonfig-0.1.2/emkonfig/registry.py
--rw-r--r--   0        0        0      168 2024-03-15 15:24:03.373331 emkonfig-0.1.2/emkonfig/utils.py
--rw-r--r--   0        0        0     3104 2024-05-06 14:24:16.527696 emkonfig-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 emkonfig-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-02-29 13:39:01.443391 emkonfig-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 15:33:07.236309 emkonfig-0.1.3/emkonfig/__init__.py
+-rw-r--r--   0        0        0     1759 2024-05-10 14:02:15.140274 emkonfig-0.1.3/emkonfig/config.py
+-rw-r--r--   0        0        0    13274 2024-05-10 13:53:23.825055 emkonfig-0.1.3/emkonfig/external/hydra/__pycache__/instantiate.cpython-310.pyc
+-rw-r--r--   0        0        0    18019 2024-05-10 13:51:38.329335 emkonfig-0.1.3/emkonfig/external/hydra/instantiate.py
+-rw-r--r--   0        0        0     4828 2024-05-09 13:32:22.917539 emkonfig-0.1.3/emkonfig/parsers.py
+-rw-r--r--   0        0        0     1052 2024-03-21 15:44:31.173249 emkonfig-0.1.3/emkonfig/registry.py
+-rw-r--r--   0        0        0      621 2024-05-10 14:07:27.700246 emkonfig-0.1.3/emkonfig/utils.py
+-rw-r--r--   0        0        0     3104 2024-05-10 14:08:36.768578 emkonfig-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 emkonfig-0.1.3/PKG-INFO
```

### Comparing `emkonfig-0.1.2/emkonfig/config.py` & `emkonfig-0.1.3/emkonfig/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,7 +38,13 @@
         if content is None:
             content = self.original_yaml_content
 
         new_content = content.copy()
         for syntax in self.parse_order:
             new_content = self.syntax_to_parser[syntax].parse(new_content, new_content)
         return OmegaConf.create(new_content)
+
+    def print(self, config: DictConfig) -> None:
+        print(OmegaConf.to_yaml(config))
+
+    def __repr__(self) -> str:
+        return OmegaConf.to_yaml(self.parse())
```

### Comparing `emkonfig-0.1.2/emkonfig/parsers.py` & `emkonfig-0.1.3/emkonfig/parsers.py`

 * *Files identical despite different names*

### Comparing `emkonfig-0.1.2/emkonfig/registry.py` & `emkonfig-0.1.3/emkonfig/registry.py`

 * *Files identical despite different names*

### Comparing `emkonfig-0.1.2/pyproject.toml` & `emkonfig-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emkonfig"
-version = "0.1.2"
+version = "0.1.3"
 description = "YAML template based configuration management tool"
 authors = ["Kıvanç Yüksel <kivanc.yuksel@emkademy.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers= [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `emkonfig-0.1.2/PKG-INFO` & `emkonfig-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emkonfig
-Version: 0.1.2
+Version: 0.1.3
 Summary: YAML template based configuration management tool
 License: MIT
 Author: Kıvanç Yüksel
 Author-email: kivanc.yuksel@emkademy.com
 Requires-Python: >=3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

