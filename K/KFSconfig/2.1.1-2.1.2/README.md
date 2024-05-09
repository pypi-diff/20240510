# Comparing `tmp/kfsconfig-2.1.1.tar.gz` & `tmp/kfsconfig-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsconfig-2.1.1.tar", max compression
+gzip compressed data, was "kfsconfig-2.1.2.tar", max compression
```

## Comparing `kfsconfig-2.1.1.tar` & `kfsconfig-2.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    15698 2024-05-06 13:39:07.358190 kfsconfig-2.1.1/KFSconfig/KFSconfig.py
--rw-r--r--   0        0        0      514 2024-05-06 13:39:07.358190 kfsconfig-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      668 2024-05-06 13:39:07.358190 kfsconfig-2.1.1/readme.md
--rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 kfsconfig-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    15698 2024-05-09 22:29:04.382243 kfsconfig-2.1.2/KFSconfig/KFSconfig.py
+-rw-r--r--   0        0        0      514 2024-05-09 22:29:04.382243 kfsconfig-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0      668 2024-05-09 22:29:04.382243 kfsconfig-2.1.2/readme.md
+-rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 kfsconfig-2.1.2/PKG-INFO
```

### Comparing `kfsconfig-2.1.1/KFSconfig/KFSconfig.py` & `kfsconfig-2.1.2/KFSconfig/KFSconfig.py`

 * *Files identical despite different names*

### Comparing `kfsconfig-2.1.1/pyproject.toml` & `kfsconfig-2.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 authors     = ["9FS <pray4spam@googlemail.com>"]
 description = ""
 license     = "MIT"
 name        = "KFSconfig"
 packages    = [{ include = "KFSconfig" }]
 readme      = "readme.md"
 repository  = "https://github.com/9-FS/2023-09-20-KFSconfig"
-version     = "2.1.1"
+version     = "2.1.2"
 
 [tool.poetry.dependencies]
-kfslog = "^1.0.0"
+kfslog = "^2.0.0"
 python = "^3.12.0"
 
 [tool.poetry.group.dev.dependencies]
 hypothesis = "^6.0.0"
-pytest     = "^7.0.0"
+pytest     = "^8.0.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires      = ["poetry-core"]
```

### Comparing `kfsconfig-2.1.1/readme.md` & `kfsconfig-2.1.2/readme.md`

 * *Files identical despite different names*

### Comparing `kfsconfig-2.1.1/PKG-INFO` & `kfsconfig-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: KFSconfig
-Version: 2.1.1
+Version: 2.1.2
 Summary: 
 Home-page: https://github.com/9-FS/2023-09-20-KFSconfig
 License: MIT
 Author: 9FS
 Author-email: pray4spam@googlemail.com
 Requires-Python: >=3.12.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: kfslog (>=1.0.0,<2.0.0)
+Requires-Dist: kfslog (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/9-FS/2023-09-20-KFSconfig
 Description-Content-Type: text/markdown
 
 ---
 Topic: "KFSconfig"
 Author: "구FS"
 ---
```

