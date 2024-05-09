# Comparing `tmp/kfslog-1.1.1.tar.gz` & `tmp/kfslog-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfslog-1.1.1.tar", max compression
+gzip compressed data, was "kfslog-2.0.0.tar", max compression
```

## Comparing `kfslog-1.1.1.tar` & `kfslog-2.0.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0    17246 2023-10-03 10:09:33.872181 kfslog-1.1.1/KFSlog/KFSlog.py
--rw-r--r--   0        0        0        0 2023-10-03 10:09:33.872181 kfslog-1.1.1/KFSlog/__init__.py
--rw-r--r--   0        0        0      561 2023-10-03 10:09:33.872181 kfslog-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      631 2023-10-03 10:09:33.872181 kfslog-1.1.1/readme.md
--rw-r--r--   0        0        0     1130 1970-01-01 00:00:00.000000 kfslog-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    25385 2024-05-09 22:13:13.920913 kfslog-2.0.0/KFSlog/KFSlog.py
+-rw-r--r--   0        0        0      581 2024-05-09 22:13:13.920913 kfslog-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      631 2024-05-09 22:13:13.920913 kfslog-2.0.0/readme.md
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 kfslog-2.0.0/PKG-INFO
```

### Comparing `kfslog-1.1.1/pyproject.toml` & `kfslog-2.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 authors     = ["9FS <pray4spam@googlemail.com>"]
 description = ""
 license     = "MIT"
 name        = "KFSlog"
 packages    = [{ include = "KFSlog" }]
 readme      = "readme.md"
 repository  = "https://github.com/9-FS/2023-09-20-KFSlog"
-version     = "1.1.1"
+version     = "2.0.0"
 
 [tool.poetry.dependencies]
 colorama = { version = "^0.4.6", optional = true }
 kfsfstr  = "^1.1.0"
 python   = "^3.12.0"
+result   = "^0.16.0"
 
 [tool.poetry.group.dev.dependencies]
-hypothesis = "^6.87.0"
-pytest     = "^7.4.2"
+hypothesis = "^6.0.0"
+pytest     = "^8.0.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires      = ["poetry-core"]
```

### Comparing `kfslog-1.1.1/readme.md` & `kfslog-2.0.0/readme.md`

 * *Files identical despite different names*

### Comparing `kfslog-1.1.1/PKG-INFO` & `kfslog-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: KFSlog
-Version: 1.1.1
+Version: 2.0.0
 Summary: 
 Home-page: https://github.com/9-FS/2023-09-20-KFSlog
 License: MIT
 Author: 9FS
 Author-email: pray4spam@googlemail.com
 Requires-Python: >=3.12.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: kfsfstr (>=1.1.0,<2.0.0)
+Requires-Dist: result (>=0.16.0,<0.17.0)
 Project-URL: Repository, https://github.com/9-FS/2023-09-20-KFSlog
 Description-Content-Type: text/markdown
 
 ---
 Topic: "KFSlog"
 Author: "구FS"
 ---
```

